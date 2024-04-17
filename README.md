# Overview

A collection of pull request guidelines, tips, and practices that help guide conversations for teams.

## Considerations

 - Decide if you really *want* to draw the authors attention 
 - decide if you really *need* the change - if not, a tech-debt story is an option, too
 - Petty comments trigger emotions

> strong opinions weakly held  
> strong opinions strongly held
[Code Review Guidelines for Humans](https://phauer.com/2018/code-review-guidelines/)


## Team Norms
- Align on *how* the team leaves feedback

### Norms to consider
- Log disagreements - time provides perspective
  - review like retros
- Why do we care about fixing code in PR's?
  - It's expensive to fix later
- Quality Tests
  - Excellent tests make changing code cheaper

## Avoid Conflicts
- Implement lint - these conflicts are annoying when style can be automated
- Emojis can indicate strong opinions, weekly held - lets discuss over 🍺
- Consider focusing on tests - maybe in lieu of coding style?
  - Does the test make sense?
    - I can read and understand the intent
    - The test explains the use-case or business rule being tested
  - Are important use-cases covered?


## Feedback Considerations
Topics to consider when leaving feedback

### Conflict Resolution
- Do not block working code
  - Allow the code to merge to better-serve users/customers.
  - Follow up with logging the disagreements, google-docs, for example. Review disagreements on a regular basis - time gives perspective.
-   [Creating a pull request template for your repository](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/creating-a-pull-request-template-for-your-repository)
    -   Checklist of agreed upon items that will be included to receive feedback

> 🎙️ PODCAST: [‎Coding Blocks: Google's Engineering Practices - Code Review Standards](https://podcasts.apple.com/us/podcast/coding-blocks/id769189585?i=1000474195476)

 
### Considerations
Purpose: To ensure quality of code over time
- How much time to spend?
- What to look for when keeping high code quality
  - Design - is the code well-designed and appropriate for the system?
    - Are the design patterns used effectively?
    - Is there already a method created for this code?
    - Why use integer here when everything else is XXX?
  - Code behavior
    - Does this fulfill the features requirements?
  - Complexity
    - Could the code be made simpler?
    - Would another developer be able to easily understand the code?
  - Tests
    - Does the code have correct and well-designed tests?
  - Naming
    - Did the developer choose good names for classes, methods, etc?
    - Alignment on naming things like `x` and `xxxHelper`
  - Comments
    - Are the comments clear and useful?
    - Prefer well-named methods over comments
  - Style Guide 
    - Should be followed - is the deviation necessary?
    - lint should fail builds
  - Documentation
    - Had documentation been created or updated?
  - Choosing the right reviewer
    - Someone who can give the most-thorough review, within the time-frame
    - When PR is low priority - give time for all team to review
    - When pr is high priority - 
    - Different people may have better understandings
