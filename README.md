# helloworld-web3-app
Basic helloworld app using web3 technologies

# Running the app

### Pre-requisites

In order to run this app, you'll need an account with the following services

- [Alchemy](https://www.alchemy.com/)
- [Metamask](https://metamask.io/)

# Dependencies

Create a new `.env` in the project root, which will will contain your alchemy endpoint, and Metamask private key

```
API_URL="EXAMPLE_URL"
PRIVATE_KEY="EXAMPLE_KEY"
```

Then run, `npm install` to install the dependencies

# Deploying a contract

In order for a contract to be deployed, it must first be compiled by running `npx hardhat compile`.

Next, run `npx hardhat run scripts/deploy.js --network ropsten`

You should then see an output message, containing the contract address and the from (wallet) address

```
Contract deployed to address: <CONTRACT> from: <WALLET>
```

You can verify this on the Ropsten Network: https://ropsten.etherscan.io/address/<WALLET_ADDRESS>

and in Alchemy: https://dashboard.alchemyapi.io/explorer?time_min=1633899574104&time_range_preset=last5Minutes
