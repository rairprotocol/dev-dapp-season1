## 6. EVM Deploy
RAIR comes with built-in smart contracts, and while you are free to use your own, we built in a lot of cool features 

## Pre-Configuration
### 1. Etherscan API Key
Register on [Etherscan](https://etherscan.io/) to get an API key. You'll need this for your .env configuration.
### 2. CoinmarketCap API key
Register on [CoinMarketCap](https://coinmarketcap.com/) to get an API key. You'll need this for your .env configuration.
### 3. Alchemy RPC Node
If you did the last task you'll already have your free RPC node. If you have not done the last task, see the previous documentation [5. Modify Dapp](https://github.com/rairprotocol/dev-dapp-season1/blob/main/Season%201%20Tasks/5.%20Modify%20Dapp/README.md) for instructions on how to get your RPC node set up. Note, your alchemy node has a different address for both Mainnet and Testnet. You'll find both in your dashboard.
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
First we need to compile all the contracts and make sure the environment values are working correctly. We have included a script to do this. 
1. In your IDE, from the root of the ```RAIR-Solidity``` repository, navigate to ```diamond-contracts```.
2. Run ```nvm use``` to read the ```.nvmrc``` file in the folder and install the appropriate Node version.
3. Run ```npm i``` to install all the necessary packages.
4. Locate and copy ```sample.env```. Rename the copy to ```.env```. 
5. Open ```.env```. We will need to populate 4 values:
   - ```ETH_MAIN_RPC=``` Is the address of your Mainnet RPC Node. This is used for the test script and uses no fees.
   - ```SEPOLIA_RPC=``` Is the address of your Testnet RPC Node. We will deploy our contract to Sepolia Testnet since we can use a sepolia faucet to pay for the transaction fees.
   - ```ADDRESS_PRIVATE_KEY=``` Is the private key of the wallet which will deploy the contract. DO NOT share this private key with anyone for any reason. DO NOT commit code with your private keys exposed in plaintext. We will never ask you to send us your private key, and you should remove your private key permanentely from this file after completing the task.
   - ```ETHERSCAN_API_KEY=``` For verifying contract deployment.
7. Save ```.env```
8. Locate ```hardhat.config.js```
9. On line 43, change ```blockNumber``` to ```21876874```
10. Scroll down to line 75. Comment out the block related to ```MINATO_RPC``` as this currently causes an error.
11. Save ```hardhat.config.js```
12. In the terminal, navigate to ```diamond-contracts```. Run the command ```npm run test```, this will compile all contracts and make sure the environment values are working correctly.

If everything works out we can move on to the next step. Its ok if there are a few errors, but if there are hundreds or it doesnt compile you might want to go back and double-check the previous steps. Next we are going to deploy the contracts to Sepolia Testnet.

13. 
14. Navigate to the [Issues](https://github.com/rairprotocol/dev-dapp-season1/issues) tab in the dev-dapp-season1 repository
15. Click "New Issue" (the green button).
16. Add a title to your issue. In this case your title should read "2. Favorite EIP"
17. Copy-paste the text below in the body of your new issue, and edit it according to our requests.
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

