# Plan

## UI

- Translations
  - [ ] translations
- More
  - [ ] pair
  - [x] wrap
  - [x] auto
- Filters
  - [x] disable_group
  - [x] blacklist
- File Modifiers
  - backup_file
  - replace_words
  - [x] delete_lines
- Paths
  - [x] translation_file
  - [x] execute
- [x] Json

## Events

## UI

- Paths
  - backup_file
  - translation_file
  - execute
- File Manipulation
  - replace_words
  - delete_lines
- Filters
  - disable_group
  - blacklist
- Translations
  - translations
  - pair
  - wrap
  - auto
- Json
  - onJsonUpdate

## Fields

- backup_file
  - Label and Input <https://mui.com/material-ui/react-text-field/>
- translation_file
  - Label and Input
- execute
  - String List

- replace_words
  - List of Map
- delete_lines
  - String List

- disable_group
  - String List / Autocomplete checkboxes <https://mui.com/material-ui/react-autocomplete/#checkboxes>
- blacklist
  - String List
- translations
  - List of Translation
    - Group
      - Label and Input
    - Patterns
      - String List
    - Print
      - Label and Input
    - Variables
      - List of Variable
        - Starts with
        - Ends with
    - Enable
      - Yes/No <https://mui.com/material-ui/react-checkbox/>
      - <https://mui.com/material-ui/react-switch/>
- pair
- wrap_text_post
  - Label and TextField
- wrap_text_pre
  - Label and TextField
- auto_new_line
  - Yes/No

Add Button - <https://mui.com/material-ui/react-floating-action-button/>

## Technology

React Material > webpack

<https://github.com/krishheii/ReactAppToHtml>

<https://mui.com/material-ui/getting-started/>

<https://react-bootstrap.netlify.app/docs/layout/grid>

- [x] Create project
- [x] install dependencies
- [x run `yarn start`
- [x] run `yarn build`
- [x] run html in build directory
  - [x] an additional slash in scripts tag is breaking html load
    - [x] <https://medium.com/@ns-tech-learn/how-to-install-webpack-and-configure-in-react-js-88b4b0bd0af9>
    - [x] <https://www.youtube.com/watch?v=F0ep7CTn5K8>
- [x] Explore more on the UI components available from Material
- [x] Take screenshots of components and design the wireframe
- [x] Implement the wireframe in the project
- [x] Check yarn build once more for any braking changes
- [x] Write logic to show the json contents for basic input fields
  - [x] Read react
    - [x] Props are immutable, so you need states as global
    - [x] Keys are important for data
    - [x] When state gets updated, the components are re-rendered
    - [x] dataStore state at the app level
    - [x] treat any JavaScript object that you put into state as read-only.
    - [x] Passing data deeply with context
  - [x] When json is updated update all the fields
  - [x] Have a global class to manage data store
  - [x] When a field changes directly update the data store
  - [x] Update JSON when the data store gets updated
- [x] Continue further only if json contents are capturable
  - [x] Need to do manual deep copy
  - [x] Need to introduce "Apply" button., Apply to change and show parse errors
- [x] Copy add delete from todo list app in examples
- [x] Add a component for two input fields with Array Provider
- [x] Copy json button
- [x] Prioritize bugs
- [x] Build and check
- [x] Fix major ones
- [ ] Electron app
- [x] Feature: Add provision to add new translation
- [x] Feature: Translations must be deletable
- [x] UI needs to be compactUI to be redesigned
- [x] since many translations are there not able to differentiate when the next one starts
- [x] UI shall allow shrinking translations
- [x] Feature: Different views for seeing translations
- [x] Find best way to add help in each section
- [x] Find best way to add translation help
- [x] Confirmation before translation delete
- [ ] Feature: UI shall allow reordering
  - [x] Drag drop with <https://dndkit.com/>  
- [ ] Bug: Show alert in a modern format with close button
- [x] Edit button on array provider is opening an input field, make it modern
- [x] Patterns and variables drag drop context update
- [x] PairArrayProvider formatting with box
- [x] PairArrayProvider drag and drop
- [x] Make search and replace as a list
- [ ] Add help for translations
- [ ] Add help for special variables
- [ ] Add examples for translations - build a configuration with the user, show the end result
- [ ] Add filter by group and translation print option to translations pane
- [ ] Add a pane for pair configuration
- [ ] Enable drag and drop for translations
- [ ] Refactor

## Translation Configuration Help

1. Basic sequence
2. Pattern matching
3. Capturing variables
4. Capturing multiple variables
5. Placing variable values
6. Variable capture at the ends
7. disable
8. disable a group
9. blacklist a line
10. Handling duplicates
    1. Default handling
    2. Removing all duplicate entries
    3. Removing subsequent duplicate entries
    4. Counting duplicates
    5. Counting subsequent duplicate entries
11. Auto new line
12. Wrap text
