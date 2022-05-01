## CrowdCoin

CrowdCoin is a project that I built by following tutorial on Udemy by Stephen Grider. You can find this tutorial here --> [Ethereum and Solidity: The Complete Developer's Guide](https://www.udemy.com/course/ethereum-and-solidity-the-complete-developers-guide/)

The idea behind the project is that users can create a campaign for their startup idea for example and then other users can contribute money to the campaign. And whenever the founder of the campaign needs certain amount of money for business expenses, the founder can create a request which has to be approved by at least half of the campaign contributors. Once the request is approved, specified amount of `ETH` will be transfered to the specified wallet address.

## Tech Stack

The contract is written using `Solidity`. The front-end is written with `JavaScript` using `Next.js` framework.

## !!! Very important !!!

In the `dev.sh` script you will add your mnemonic, so please make sure that you do not accidentally push it to your git or somewhere else. Keep it private at all times. The `dev.sh` script is added to `.gitignore` so it won't be pushed to the repo, but still be very careful.

## How to run the app

To install all dependencies run `npm install`.

To run the app you will need to create the following `.sh` scripts:

- `dev.sh` - in this script specifiy the following - `export MNEMONIC="add your mmemonic here" && export RINKEBY="add your infura url to Rinkeby" && export CONTRACT_ADDRESS="add your contract address here" && npm run dev `
- `deploy.sh` - in this script specifiy the following - `export MNEMONIC="add your mmemonic here" && export RINKEBY="add your infura url to Rinkeby" && node ethereum/deploy.js`

First you will have to deploy the smart contract by using the `deploy.sh` script which will deploy the contract and will print out the conract address. And then add that address of the contract as env var to the `dev.sh` script and run it. This will start the app.

You can run these scripts manually or just run the `make dev` and / or `make deploy` commands.

Once the app is running, go to `localhost:3000` and play around with the app, have fun :) And let me know if you have any questions.

## Metamask

Make sure you have Metamask installed and that you have `ETH` on your account on `Rinkeby` test network.

## Screenshots
