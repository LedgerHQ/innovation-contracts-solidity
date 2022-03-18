# innovation-contracts-solidity

Collection of smart contracts written in Solidity

This repository contains smart-contract used by Ledger. For example we might add a ERC721 ugradeable based on solmate that would be used by other project. 

## Install

To get all npm packages

    npm install

To get all git modules dependencies

    forge update

In case you have VSCode path issue. The file is in .gitignore because path are absolute 

    forge remappings > remappings.

## Git hooks

We use [lefthook](https://github.com/evilmartians/lefthook) to manage our git hooks. For the moment, the following hooks are configured:
- Run `npm run prettier` before pushing to remote
- Run `forge test` before pushing to remote

### How to install

You only need to do this step once. Run `npx @arkweid/lefthook install` in the root of the repository to install the git hooks described in the `lefthook.yml` file.

## How to run manually

You can manually run the installed git hooks by running `npx @arkweid/lefthook run pre-push` or by running the alias defined in the `package.json` file (`npm run lefthook`).
