# @nationalgrid-engineering/frontend-libraries

This Repository is a monorepo that is managed by [Turborepo](https://turbo.build/repo) and contains multiple packages for frontend consumption.

### Pre-requisites

Before running the below commands install homebrew (Homebrew is a software package management system) from self-service just in case the commands don't work.

This repository's NodeJS version is managed by [NVM](https://github.com/nvm-sh/nvm) (Node Version Manager). If you don't already have NVM installed, you can run `brew install nvm` to install it. Once installed you can run `nvm use` which will provide you instructions to install the correct version of Node if it is not already installed. If it is already installed, the correct node version will be selected for the project.



### Setup Github & NPM regristry credentials
Step 1: Ensure that you have an ssh key configured for your github account so then you are able to clone the repository locally by following [this tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account).

Once your ssh key has been created in github, Click the "Configure SSO" button for the key and ensure that the key is authorised for `nationalgrid-engineering`

Step 2: open or create your user-level npm config at `~/.npmrc` and copy the below into the file
Note: for mac, if hidden files are not visible, press [`CMD` + `Shift` + `.`] then you will be able to see/create your `.npmrc` file.

```bash
//npm.pkg.github.com/:_authToken=[YOUR_ACCESS_TOKEN]
```

Step 3: Generate a [Personal Access Token (classic)](https://github.com/settings/tokens) with at least read:package selected in the available scopes.

Step 3: copy your new token and replace [YOUR_ACCESS_TOKEN] in your user-level `.npmrc` file with your new token. (you will not be able to see the token again after leaving this github page)

Step 4: Click the "Configure SSO" button on your newly created token and select `nationalgrid-engineering`

## Getting Started

Step 5: Installing Dependencies

Install dependencies by running `npm i`
Install husky git hooks `npm run prepare`

run `npm run dev` which will start storybook and add run watchers to build the packages when they change so then changes are reflected in storybook.

### Git hooks

This repository uses [husky](https://typicode.github.io/husky/#/) to apply commands to git hooks:

- pre-commit uses [lint-staged](https://github.com/okonet/lint-staged) to fix any linting errors of your staged changes
- pre-push runs the test command to ensure all jest based tests are passing before being pushed
- commit-mgs uses [commitlint](https://commitlint.js.org/#/) to lint commit messages to ensure conventional commit messages are enforced.
  for more information on conventional commit messages and how to construct them, click [here](https://www.conventionalcommits.org/en/v1.0.0/)
