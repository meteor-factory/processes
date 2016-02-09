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

Devs should:
* Keep Trello board in sync with their work

#### Columns
* **Ideas** - Tasks that might be done
* **Backlog** - Tasks that should eventually be done
* **Todo / Sprint [date]** - The next set of tasks to be done / completed for the end of the sprint
* **In progress** - Tasks that are actively being worked on
* **Pull Request** - A PR has been created in Github
* **Testing MF** - To be tested by Meteor Factory project manager
* **Testing** - To be tested by the client
* **Tested** - Passed by the client

#### Assigning
The active developer should be assigned to the card. This means that you're responsible for the card and are 'blocking' the cards completion.

* Assign yourself to the cards you're working on
* If you're waiting for mockups etc. assign the designer / move the card to backlog
* Assign yourself to cards that you'd be good at (e.g. worked on before)
* Try not to overassign yourself, as it may stop other devs from jumping on the card

#### Pull Requests
The senior devs in each project are responsible for accepting PRs.

Once a PRs is accepted the latest code should be deployed to the staging url so it can be tested.

#### Testing
Tickets are only allowed to be moved into testing when they are running live on the staging url.

When a card passes, it is moved into the next column.

When a card fails, it should receive the label 'Failed Test' and be moved into the 'To do / Sprint' column

#### Labels
Labels can be created where useful.

Most common labels:
* Bug
* Failed test

## Slack
Slack should be used for instant chat between devs, client and project manager.

Project manager should:
* Set up slack channel
* Invite devs
* Invite client

Commonly needed project files like trello link or hour sheets will be stored in the header of the main channel.


## Github
Project manager should:
* Set up private Github repo
* Invite devs
* Invite client (where appropriate)
* Set default branch to `develop` (once it's been pushed)

For more, see [Committing Code](https://github.com/meteor-factory/processes/blob/master/Comitting%20Code.md)
