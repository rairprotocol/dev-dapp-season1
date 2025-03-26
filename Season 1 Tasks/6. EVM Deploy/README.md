## 6. EVM Deploy
Ethereum Virtual Machine (EVM) is a distributed state machine which allows for the execution of arbitrary code via Smart Contracts. Smart contracts are simply chunks of code deployed to a specific address where they can be called on to execute functions for a user who pays a transaction fee. Very cool stuff.

RAIR comes with built-in Diamond Smart Contracts. What's a Diamond Smart Contract you ask? It's akin to a modular engine. This design allows for seamless upgrades and maintenance without overhauling the entire system. Given that once a contract has been deployed, it cannot ever be changed, Diamond archetecture allows us to graft new components and features to an already deployed contract, expanding its capabilities while maintaining its persistence.

In this task we will show you how to deploy your own RAIR Diamond Contracts to Sepolia Testnet. Its a little more involved than the others before it so pay close attention to the instructions. By the end you'll have a set of contracts deployed which you own! 

## Pre-Configuration
### 1. Etherscan API Key
Register on [Etherscan](https://etherscan.io/) to get an API key. You'll need this for your .env configuration.
### 2. CoinmarketCap API key
Register on [CoinMarketCap](https://coinmarketcap.com/) to get an API key. You'll need this for your .env configuration.
### 3. Alchemy RPC Node
If you did the last task you'll already have your free RPC node. If you have not done the last task, see the previous documentation [5. Modify Dapp](https://github.com/rairprotocol/dev-dapp-season1/blob/main/Season%201%20Tasks/5.%20Modify%20Dapp/README.md) for instructions on how to get your RPC node set up. Note, your alchemy node has a different address for both Mainnet and Testnet. You'll find both in your dashboard.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/1.png" width="50%"/>

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

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/2.png" width="25%"/>

2. Run ```nvm use``` to read the ```.nvmrc``` file in the folder and install the appropriate Node version.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/3.png" width="25%"/>

3. Run ```npm i``` to install all the necessary packages.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/4.png" width="25%"/>

4. Locate and copy ```sample.env```. Rename the copy to ```.env```. 

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/5.png" width="25%"/>

5. Open ```.env```. We will need to populate 4 values:
   - ```ETH_MAIN_RPC=``` Is the address of your Mainnet RPC Node. This is used for the test script and uses no fees.
   - ```SEPOLIA_RPC=``` Is the address of your Testnet RPC Node. We will deploy our contract to Sepolia Testnet since we can use a sepolia faucet to pay for the transaction fees.
   - ```ADDRESS_PRIVATE_KEY=``` Is the private key of the wallet which will deploy the contract. DO NOT share this private key with anyone for any reason. DO NOT commit code with your private keys exposed in plaintext. We will never ask you to send us your private key, and you should remove your private key permanentely from this file after completing the task.
   - ```ETHERSCAN_API_KEY=``` For verifying contract deployment.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/6.png" width="25%"/>

7. Save ```.env```
8. Locate ```hardhat.config.js```

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/7.png" width="25%"/>

9. On line 43, change ```blockNumber``` to ```21876874```

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/8.png" width="50%"/>

10. Scroll down to line 75. Comment out the block related to ```MINATO_RPC``` as this currently causes an error.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/9.png" width="25%"/>

11. Save ```hardhat.config.js```
12. Make sure you're in the ```/diamond-contracts``` folder. In the terminal, run the command ```npm run test```, this will compile all contracts and make sure the environment values are working correctly.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/10.png" width="25%"/>

If everything works out we can move on to the next step. Its ok if there are a few errors, but if there are hundreds or it doesnt compile you might want to go back and double-check the previous steps. Next we are going to deploy the contracts to Sepolia Testnet.

13. We need to modify ```ERC20.js``` in ```/diamond-contracts/deploy``` with the public key of our wallet. This will make us the owner of the contract and give us the permissions to mint new tokens on the contract should we wish.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/11.png" width="25%"/>

14. Uncomment line 13 and paste your public address between the quotes. Save the file.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/12.png" width="50%"/>

15. From ```/diamond-contracts``` run ```npx hardhat --network 0xaa36a7 deploy```. It will take some time to fully deploy all the contracts.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/13.png" width="50%"/>

16. You should eventually see all the contract addresses.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/14.png" width="50%"/>

Congratulations! You have deployed all the RAIR smart contracts to Sepolia Testnet. These are your contracts, you own them! Use these contracts to test transactions on your own Dapp so long as you have SepoliaETH in your wallet. When you are ready for a mainnet deployment you can deploy a new set of contracts on any EVM-compatable blockchain you wish. 

To round things out we just need to create a new issue:

17. Navigate to the [Issues](https://github.com/rairprotocol/dev-dapp-season1/issues) tab in the dev-dapp-season1 repository
18. Click "New Issue" (the green button).
19. Add a title to your issue. In this case your title should read "6. EVM Deploy"
20. Copy-paste the text below and add the [Sepolia Etherscan](https://sepolia.etherscan.io) link of your deployed ```RAIR20``` contract.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/15.png" width="50%"/>
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/6.%20EVM%20Deploy/16.png" width="50%"/>

```
My RAIR20 Etherscan link is [https://sepolia.etherscan.io/address/0xAddress].
```
6. Click "Create" (the green button)

Upon completion, your task will be validated and if it is correct, you will be assigned the "EVM Deploy" label. If there is an issue, you will see the "Unresolved" label, this means there is a problem that needs to be corrected. Edit your issue and follow the guidelines more closely until you receive your "EVM Deploy" label. Do not create multiple issues for the same task. If you dont see your issue, it means it has been validated and closed. Verify this by setting the sort settings to show closed issues.

Congratulations! Continue with the next task to earn levels and climb the leaderboard to earn your share of the rewards!

## Recommended Reading 
[Juan's Hardhat Guide for Deploying Smart Contracts](https://github.com/rairprotocol/rair-solidity/blob/main/GUIDE.MD)\
[Ethereum Virtual Machine (EVM)](https://ethereum.org/en/developers/docs/evm/)

## Labels
Label Awarded: "EVM Deploy"\
Sponsor: None
