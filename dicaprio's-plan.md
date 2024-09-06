# The plan

## Step 1

- work out how to run linting `npm run lint` 🍸
- install Husky `npm install --save-dev husky` 🍸
- `npx husky init` makes a script and updates script in package.json to create a pre-commit hook 🍸
- try commit and make husky lit check🍸
- Change the code to give you a warning/error 🍸
- Use git log to see if the commit completed or was stopped🍸
- make the linter more strict, change the npm script for linting so even warnings are not allowednp🍸

## Step 2

- Install prettier as a dev dependency🍸
- `npx prettier --write 'app/'` 🍸
- Create an npm script to run prettier 🍸
- Test that it works 🍸
- Test you can make it angry 🍸
- Add to husky pre-commit hook 🍸
- test again 🍸

## Step 3

- Create a component for the h2's that takes a title prop 🍸
  - Create a components folder 🍸
  - Create a Title component 🍸
- Test component works 🍸
- install jest
- look into and install react testing library
- create an npm test script
- write a basic test for the title component
- Test the test
  - Write component to fail
  - Test it fails
- Add test script to husky pre-commit hook
- Test the hook works
- make sure failing test stops commit

## Hackathon plan

### Objectives

- When you put in a "Pull Request" (PR) from a feature branch into the main branch there should be a Github Action that automatically runs things like linting, formatting, testing and auditing.
- You should not be able to merge a PR into main unless the steps in the Github Action (lint, format etc etc) all pass.
- You should not be able to push/merge commits directly to the main branch, everything should have to go through the PR process.
- When you merge the feature branch into the main branch this should trigger an automated workflow in Render. Render should watch for changes in your main branch, when it sees a change it will pull the code, run the Docker production build and then deploy the Next.js site. You should be able to see your Next.js app live on the internet.

### Steps

- Create a Github action
  - Create .github folder with a workflow sub folder 🍸
  - Create a yaml file (.yml) for a simple action 🍸
  - Write simple github action to echo a Leo quote on pr merge into the main branch 🍸
  - Commit to main 🍸
  - Test its working!
    - Create feature branch 🍸
    - make change and commit 🍸
    - Create pull request🍸
    - Merge PR🍸
    - Should echo leo quote🍸

- docker build and docker run in a Github Action 🍸
  - rename ymlfile
  - install docker step
  - docker build step
  - docker run step `docker run --rm image_name_here npm run lint && npm run format` 
    - with lint
    - with format
  - Test
  - Prevent merge if errors in checks
    - Set up ruleset in github to prevent merging
  - Test

