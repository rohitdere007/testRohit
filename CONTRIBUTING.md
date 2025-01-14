# Contributing to front-libraries 

Welcome to frontend-libraries, the home of the libraries that implement the National Grid Experience System (NGES). We're happy you found yourself here and are looking to contribute to the library.
Design Systems and Component Libraries are the intersection of Dev and Design, as such this repository has co-ownership from [Human Centered Design](https://teams.microsoft.com/l/team/19%3acb204ac264df43e396a7cc7713f2f1b5%40thread.tacv2/conversations?groupId=6260379d-d027-4742-87db-f69d16ec5634&tenantId=f98a6a53-25f3-4212-901c-c7787fcd3495) and [Core Software engineering](https://confluence.devops.nationalgrid.com/display/DIG/Core+Software+Engineering), we welcome and strongly encourage the community to actively collaborate and contribute to ensure these tools provide maximum value to consuming product engineering teams across the organization.

In a nutshell our contributing model is:

**Propose => Design => Code => Document**


## Table of Contents
- [Quick links](#links)
- [Scope](#scope)
- [Getting Started](#getting-started)
- [Workflow](#workflow)
  - [Propose](#propose)
  - [Design](#design)
  - [Code](#code)
  - [Document](#document)
- [Pull Requests](#pull-requests)
- [Code of Conduct](#code-of-conduct)

## Quick Links
- **Docs**: [StoryBook](https://curly-telegram-9ko6qwn.pages.github.io/)
- **Issues**: [Open Issues](https://github.com/nationalgrid-engineering/frontend-libraries/issues)
- **Project**: [Kanban board](https://github.com/orgs/nationalgrid-engineering/projects/2/views/1)

## Scope

Some example use cases for contribution

- Error in the example code
- Updated packages / actions required
- Different approaches to achieve the same task
- New features in the libraries such as a new component at atom or molecule level
- Requesting a product component shared across different codebase's be graduated to the library for enhanced re-use.

As always, reach out to Core Engineering on our [teams channel](https://teams.microsoft.com/l/channel/19%3aNaU050QowgMBk00rpE19xJ-gSLI1kczvwpDvvWuNiOE1%40thread.tacv2/General?groupId=f42effac-8ba7-42bc-9137-f892208931a5&tenantId=f98a6a53-25f3-4212-901c-c7787fcd3495) if you would like guidance, discussion, or if you would like to pair program your PR! For design related questions, Human Centered Design have a [dedicated teams channel for the Design System](https://teams.microsoft.com/l/team/19%3acb204ac264df43e396a7cc7713f2f1b5%40thread.tacv2/conversations?groupId=6260379d-d027-4742-87db-f69d16ec5634&tenantId=f98a6a53-25f3-4212-901c-c7787fcd3495).


## Getting Started
- Clone the repo and follow the steps outlined in the README.md
- Install dependencies by running `npm i`.
- Run `npm run dev` to run Storybook locally & package watchers

## Workflow for contributions
Our workflow is divided into four major steps: **Propose, Design, Code, and Document**. 

### Propose

- Use the GitHub associated with this repo to start a new feature request. Please reach out to the [CSE team](https://github.com/orgs/nationalgrid-engineering/teams/principal-engineers) at this time. You'll be invited to the next regular Sync session for the library to chat through your proposal and case with the team. 

- Articulate feature direction, scope, and related ideas. Ensure that you engage with your teams lead designer. If they have pending question on the NGES design system please reach out to **Andrew Darkins** in [HCD](https://teams.microsoft.com/l/team/19%3acb204ac264df43e396a7cc7713f2f1b5%40thread.tacv2/conversations?groupId=6260379d-d027-4742-87db-f69d16ec5634&tenantId=f98a6a53-25f3-4212-901c-c7787fcd3495).

- Finalize scope and plan next steps.
    - Document as a TODO card in the [GitHub Project](https://github.com/orgs/nationalgrid-engineering/projects/2/views/1)

### Design (Lead by Andrew Darkins)

- Designs and sign-off from HCD are needed in the case of a new component. If it's a code only modification the design step will be covered in a sync call.

- The design team will review designs from your product designer and add to the source Figma doc.

- The design team will test for accessibility.

- The design team will use one of the recurring design only sessions to review the design with the developer/product person or appropriate team representative. 

### Code

- Create a new branch and set up your environment.

- Create the component or modification in question, this can be done either directly in Storybook or using one of the example Apps to experiment with behavior. 

- Conduct functionality, browser, and accessibility tests.

- Code review by peers. The CSE team will review the PR.

- Check-in and chat through changes with approvers on a regular sync call (if necessary).

### Document

- Familiarize yourself with the documentation format in storybook. 

- Write the documentation. 

- Peer review the documentation.

- PR the documentation along with the code changes

## Pull Requests

Contribution should be via a Pull Request

1. Clone the repository
2. Install dev dependencies by running `npm i`
3. Setup the husky pre-commit hook by running `npm run prepare` which will lint your changed on commit
4. Create a new feature branch with a name of `feat/<the reason for your change>`
5. Make the changes you require to that branch
6. Push your code
7. Submit a pull request with an appropriate title and detailed comments
