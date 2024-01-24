# Storybook Example Project

## General Workflow
- Add new Component
- Add Story for this Component
  - A story are one or more usages of this component. Examples
    - Story 1: Button with props "variant: Primary"
    - Story 2: Button with props "variant: Secondary"
    - Story 3: Button with props "icon: add"
  - Add tests to each story (optional)
    - Story 1 Example: Test that the color is "blue"
  - Commit the changes
  - Create a PR: See here: https://github.com/jannikwienecke/l21s-example-storybook/pull/1
  - Github Actions runs and publishes the storybook build to "chromatic"
  - In Chromatic, the stories and its tests are validated
  - If the changes effected the ui of any of the components, these changes can be seen, compared to the old version and approved: see here: https://www.chromatic.com/review?appId=65b12a2908ad634bdd02f982&number=1&type=linked
  - After the changes are approved, MR can be merged
