# Deploying
A developer should be in charge of the deployment process.

## App hosting
Currently we use Modulus for hosting. In the future we'll probably switch to Galaxy.

The developer should:
* Set up organisation `My Project` under the `myproject@gmail.com` email
* Two apps, `my-project-stage` and `my-project`

## Database Hosting
We should switch to Compose.io for Mongo Hosting

The developer should:
* Sign up for new Compose account with `myproject@gmail.com`
* Set up new MongoDB (not MongoDB+)
* Create databases `stage` and `production` and users `stage` and `production`, each with Oplog

## Continuous Integration
We are using [Codeship](codeship.com) for continuous integration.

We do this to:
* Enable deployment via `git push` to certain branches
* Enable automatic testing

Currently, Ben has to set up a project and invite devs to collaborate.

In the Codeship control panel, this following might be helpful

**Testing -> Setup Commands**
```
nvm install 5.2.0
nvm use 5.2.0
npm install jshint -g
npm install chimp -g
npm install selenium-standalone -g
selenium-standalone install --version=2.50.1 --baseURL=https://selenium-release.storage.googleapis.com --basePath=`npm config get prefix`/lib/node_modules/chimp/node_modules/selenium-standalone/.selenium
curl -o meteor_install_script.sh https://install.meteor.com/
chmod +x meteor_install_script.sh
sed -i "s/type sudo >\/dev\/null 2>&1/\ false /g" meteor_install_script.sh
./meteor_install_script.sh
export PATH=$PATH:~/.meteor/
cd app
```
N.B. this assumes Meteor app is in `app` subfolder of repo

**Testing -> Configure Test Pipelines**
```
meteor --settings private/settings/dev.json --port 3000 &
sleep 240 && chimp --ddp=http://localhost:3000 --path=tests --mocha --browser=chrome
```

**Deployment -> Deployment Pipelines**

Pipeline 1: `Branch should be exactly master`

Pipeline 2: `Branch should be exactly stage`
