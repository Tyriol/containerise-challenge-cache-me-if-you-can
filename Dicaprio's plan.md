# The plan

## Step 1

- work out how to run linting `npm run lint` 🍸
- install Husky `npm install --save-dev husky` 🍸
- `npx husky init` makes a script and updates script in package.json to create a pre-commit hook 🍸
- try commit and make husky lit check
- Change the code to give you a warning/error 
- Use git log to see if the commit completed or was stopped
- make the linter more strict, change the npm script for linting so even warnings are not allowednp

## Step 2

- Install prettier as a dev dependency
- Create an npm script to run prettier
- Test that it works
- Test you can make it angry
- Add to husky pre-commit hook
- test again
