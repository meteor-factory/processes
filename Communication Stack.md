# Communication Stack

The tools we primarily use for communicating are

* **Trello** - for project management
* **Slack** - for chat
* **Github** - for code

## Trello
Project manager should:
* Create a private Trello board, under the Meteor Factory organisation
* Populate with cards
* Give developers access
* Give client access
* Add link to project Github Readme

#### Columns
* **Backlog** - Tasks that should eventually be done
* **Todo** - Tasks which are decided to be done 
* ** Next Sprint [date]** - Tasks which are ready to be executed
* ** In progress** - Tasks that are actively being worked on
* **Pull Request** - A PR has been created in Github
* **Testing MF** - To be tested by Meteor Factory project manager
* **Testing** - To be tested by the client
* **Done** - Passed by the client

#### Life cycle of a card
* Project Manager, client, designer or architect creates tickets
* Tickets get normally assigned to devs (if there is no other work, devs can also take free ones)
* Devs will move their ticket to "In progress" once they start
* Devs will move their ticket to "PR" once they did a PR
* Architect will move ticket to "Testing MF" once the ticket is on staging
* Project Manager will test and move the ticket to "testing client" if it's fine or back to "failed test" / "in progress" in this case the dev wil take it again

#### Labels
Labels can be created where useful.

Most common labels:
* Bug
* Urgent
* Failed test

## Slack

Use MF Chat for all dev talk. Use Client chat basically only for communication with the client. Have in the client chat an eye on the #general channel where noticeworthy information might be shared with the client + dev team


## Github
Project manager should:
* Set up private Github repo
* Invite devs
* Invite client (where appropriate)
* Set default branch to `develop` (once it's been pushed)

For more, see [Committing Code](https://github.com/meteor-factory/processes/blob/master/Comitting%20Code.md)
