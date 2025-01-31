## 5. EVM Deploy

## Steps
1. Download the [RAIR-Solidity](https://github.com/rairprotocol/rair-solidity/tree/main) repository.
2. Install [Node Version Manager](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating). If it doesnt run after installing, follow the troubleshooting steps in the documentation.
3. From inside the RAIR-Solidity repository, navigate to ```diamond-contracts```.
4. Edit ```.nvmrc``` and decrement ```v21.2.0``` to ```v20```. Save the file.
5. Run ```nvm install``` , then ```nvm use``` to read the ```.nvmrc``` file in the folder and install the appropriate Node version.
6. Rename ```sample.env``` file to ```.env``` in the folder, fill all values (RPC endpoints, API keys, Private Key for the deployer account)
7. To test the smart contracts use the command npm run test, this will compile all contracts and make sure the environment values are working correctly. (You may need to install 
8. Navigate to the [Issues](https://github.com/rairprotocol/dev-dapp-season1/issues) tab in the dev-dapp-season1 repository
9. Click "New Issue" (the green button).
10. Add a title to your issue. In this case your title should read "2. Favorite EIP"
11. Copy-paste the text below in the body of your new issue, and edit it according to our requests.
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
