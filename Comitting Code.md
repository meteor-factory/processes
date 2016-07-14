# Committing Code

Each project will have an **architect** who's responsible for the architecture & quality of the code and **developers** working with him.

### Life cycle of a new feature:

**1. Developer**:

* `git checkout -b feature/T###-keyword` or `git flow feature start T###-keyword` (using [git flow](https://www.google.co.uk/search?q=git+flow&oq=git+flow&aqs=chrome..69i57j0l5.1034j0j1&sourceid=chrome&es_sm=119&ie=UTF-8))
  * e.g. `T143-translations` (on some projects we go without the T, this is not so important...) 
* Commit some code with message `T### : short explanation`
 * e.g. `T172: Styling for login button`
* `git push`
* Go the Github page and follow the prompts to create a new PR
* Move Trello card to "Pull Request" column

**2. Architect**:
* Check PR for code quality and consistency
* Make recommendations

**3. Developer**
* Respond to recommendations & make any changes

**4. Architect**
* Merge PR
* Move Trello card from "Pull Request" to next column
