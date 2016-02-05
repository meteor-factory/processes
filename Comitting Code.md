# Committing Code

Each project will have an **architect** who's responsible for the architecture & quality of the code.

#### Pull Requests ####
Except for very small fixes, all code should be submitted via pull request.

Life cycle of a new feature:

**1. Developer**:
* `git checkout -b feature/my-feature` or `git flow feature start my-feature` (using [git flow](https://www.google.co.uk/search?q=git+flow&oq=git+flow&aqs=chrome..69i57j0l5.1034j0j1&sourceid=chrome&es_sm=119&ie=UTF-8))
* Commit some code
* `git push`
* Go the Github page and follow the prompts to create a new PR
* Move Trello card to "Pull Request" column

**2. Architect/Senior dev**:
* Check PR for code quality and consistency
* Make recommendations

**3. Developer**
* Respond to recommendations & make any changes

**4. Architect**
* Merge PR
* Move Trello card from "Pull Request" to next column

#### Committing
* Commit messages should provide a brief summary of what you did. (`Small fixes` is OK, only if it's clear from the code changes what those fixes were)
* Commit messages should have correct spelling & grammar and always be professional
