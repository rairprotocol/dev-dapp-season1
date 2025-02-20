## 6. EVM Deploy

## Pre-Configuration
### 1. Etherscan API Key
Register on [Etherscan](https://etherscan.io/) to get an API key. You'll need this for your .env configuration.
### 2. CoinmarketCap API key
Register on [CoinMarketCap](https://coinmarketcap.com/) to get an API key. You'll need this for your .env configuration.
### 3. Alchemy RPC Node
If you did the last task you'll already have your free RPC node. If you have not done the last task, see the previous documentation [5. Modify Dapp](https://github.com/rairprotocol/dev-dapp-season1/blob/main/Season%201%20Tasks/5.%20Modify%20Dapp/README.md) for instructions on how to get your RPC node set up.
### 4. Metamask
If you did the last task you'll already have Metamask. If you have not done the last task, see the previous documentation [5. Modify Dapp](https://github.com/rairprotocol/dev-dapp-season1/blob/main/Season%201%20Tasks/5.%20Modify%20Dapp/README.md) for instructions on how to get your wallet.
### 5. Sepolia ETH
In our example, we will be deploying our smart contracts to Sepolia Testnet. This means you need Sepolia ETH to pay for the transactions. Use [Google's Sepolia Faucet](https://cloud.google.com/application/web3/faucet/ethereum/sepolia) to receive some free tokens to complete this task.
### 6. VSCode
If you already have a development environment of your own you can skip this step, but for those who dont you're gonna want to install an IDE(Integrated development environment) on your machine. IDEs are super helpful when working on large projects. They help you keep organized and provide a lot of functionality that will help in writing code easier. We recommend [VSCode](https://code.visualstudio.com/).
### 7. Clone RAIR-Solidity Repository
Head to [RAIR-Solidity](https://github.com/rairprotocol/rair-solidity) and download or clone(```gh repo clone rairprotocol/rair-solidity)``` the repository to your local machine. 
### 8. Install Node Version Manager(NVM)
You'll need a specific version of NPM installed to run the test script. In order to do this we'll use [Node Version Manager](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating). If it doesnt run after installing, follow the troubleshooting steps in the documentation.

## Steps
We are gonna start by configuring everything we need to run the test script. This includes installing packages with ```npm``` and setting the appropriate environment variables. 
1. In your IDE, from the root of the ```RAIR-Solidity``` repository, navigate to ```diamond-contracts```.
2. Run ```nvm use``` to read the ```.nvmrc``` file in the folder and install the appropriate Node version.
3. Run ```npm i``` to install all the necessary packages.
4. Locate and copy ```sample.env```. Rename the copy to ```.env```. 
5. Fill all values (RPC endpoints, API keys, Private Key for the deployer account)
6. 
7. 
8. To test the smart contracts use the command npm run test, this will compile all contracts and make sure the environment values are working correctly. (You may need to install 
9. Navigate to the [Issues](https://github.com/rairprotocol/dev-dapp-season1/issues) tab in the dev-dapp-season1 repository
10. Click "New Issue" (the green button).
11. Add a title to your issue. In this case your title should read "2. Favorite EIP"
12. Copy-paste the text below in the body of your new issue, and edit it according to our requests.
```
I checked out Ethereum Improvement Proposals! My Favorite new EIP is [Write EIP here].

The reason I like this EIP is [Write a short description why, this helps us understand what features we might want to implement in the future to our own smart contracts!]
```
6. Click "Create" (the green button)

Upon completion, your task will be validated and if it is correct, you will be assigned the "Favorite EIP" label. If there is an issue, you will see the "Unresolved" label, this means there is a problem that needs to be corrected. Edit your issue and follow the guidelines more closely until you receive your "Favorite EIP" label. Do not create multiple issues for the same task. If you dont see your issue, it means it has been validated and closed. Verify this by setting the sort settings to show closed issues.

Congratulations! Continue with the next task to earn levels and climb the leaderboard to earn your share of the rewards!

## Recommended Reading 
[Juan's Hardhat Guide for Deploying Smart Contracts](https://github.com/rairprotocol/rair-solidity/blob/main/GUIDE.MD)\
[Ethereum Virtual Machine (EVM)](https://ethereum.org/en/developers/docs/evm/)

