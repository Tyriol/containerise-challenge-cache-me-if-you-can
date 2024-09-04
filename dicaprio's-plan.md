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
