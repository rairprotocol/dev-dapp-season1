## 5. Modify Dapp
Deploy your own working Dapp using RAIR’s open-source application. RAIR includes EVM support, NFT minting, smart contracts, and streaming video with NFT DRM protection. DevDapp makes deployment easy while allowing full customization.

## Pre-Configuration
### 1. Docker
Install [Docker](https://www.docker.com/products/docker-desktop/) for containerized RAIR services.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/1.png" width="25%"/>

### 2. Alchemy
Create a free account on [Alchemy](https://alchemy.com) and sign up to get access to the dashboard. Once in the dashboard:

1. Locate "Apps" in the sidebar.

2. Create a new app.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/8.png" width="25%"/><img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/9.png" width="25%"/>

3. Choose "Ethereum" as your chain.
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/10.png" width="25%"/>

4. Activate the "Node API" service.
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/11.png" width="25%"/>

5. You will be directed to your new app. On the top right of the page you'll see your API key. You'll need this later.

6. Under "networks" you'll also see the address of your RPC node. You'll need this later as well.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/14.png" width="25%"/><img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/15.png" width="50%"/>

### 3. Metamask
Install Metamask for blockchain interactions.

### 4. VSCode
Use [VSCode](https://code.visualstudio.com/) as your development environment.

### 5. Clone RAIR
Download the [RAIR-Dapp](https://github.com/rairprotocol/rair-dapp) repository. In your IDE, run ```gh repo clone rairprotocol/rair-dapp```). 
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/2.png" width="50%"/><img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/3.png" width="25%"/>

### 6. Change Working Branch
We need to change our working branch before we start. This is necessary because later versions of RAIR-Dapp require more memory to build which may exceed your local machine's limits and cause building to fail. 

1. In VS Code locate the branch in the bottom left corrner. Click where it says "main":
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/28.png" width="25%"/>

2. This brings up the option to select a different branch of the current repository. In this case we want to use ```300-social-login-fix```
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/29.png" width="50%"/>

## Steps
We first need to configure the deployment to use your new alchemy account. We will do this by creating two ```.env``` files which contain all the variables the app might need to access before deployment. These values are referenced from these files throughout the app so they dont have to be hard-coded into the source. 
1. Locate the file in the ```Rair-Dapp-Main``` folder called ```.env.sample```
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/4.png" width="25%"/>

2. Make a copy of this file called ```.env```
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/5.png" width="25%"/>

3. Open ```.env``` and locate ```alchemy_api_key=```
4. Paste your API key from the alchemy dashboard into ```alchemy_api_key=```
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/6.png" width="25%"/>

4. Also locate ```ethereum_mainnet_rpc=``` and paste the address of your RPC node.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/27.png" width="25%"/>

5. Save your file.
6. That takes care of the backend, now we need to do the same for the frontend. Go into the ```rair-front``` folder and do the same thing with the ```.env.sample``` file in there. You wont need to change anything in here though, just rename the copy ```.env```
Deploy RAIR
7. Head back to the project root, open a terminal in VSCode. ```terminal>new terminal``` and from the repository root input ```docker compose -f docker-compose.local-new.yml up``` (ignore the -d flag in the image below).
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/18.png" width="75%"/>

8. Wait for the deployment to build. (This can take 10-15 minutes the first time around while the containers build and the database syncs with the blockchain). If you are using MacOS, there is a chance the build will fail due to a port conflict! Use [this guide](https://progressstory.com/tech/port-5000-already-in-use-macos-monterey-issue/) to free up the needed port.
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/20.png" width="25%"/>

9. If EVERYTHING IS PERFECT head to [http://localhost:8088/](http://localhost:8088/) where you will be everso kindly greeted by:
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/21.png" width="25%"/><img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/22.png" width="50%"/>

10. Locate the "Connect" button in the top-right corner. Sign in with web3 to bring up the metamask signer.

<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/23.png" width="25%"/><img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/24.png" width="25%"/>

11. Verify the transaction.
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/26.png" width="25%"/>

12. And that's it! You have successfully deployed RAIR on your local machine and connected to the Ethereum Network via your RPC node!
<img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/5.%20Modify%20Dapp/25.png" width="25%"/>

13. Pat yourself on the back.
14. Take a drink of water.
15. Now... There's still a task to finish if you want to earn levels!
16. Go to [Issues](https://github.com/rairprotocol/dev-dapp-season1/issues) tab in the dev-dapp-season1 repository
17. Click "New Issue" (the green button).
18. Add a title to your issue. In this case your title should read "5. Modify Dapp"
19. Add a screenshot of your logged in wallet on the frontend.
20. Finally copy-paste the example body text and replace [RPC Address] with the address you recieved from Alchemy.
21. Click "Create" (the green button)

## Example Body Text
```
I deployed RAIR successfully. My Alchemy RPC address is [RPC Address].
```

## Completion
Once validated, you’ll receive the "Modified Dapp" label. If issues arise, update your submission accordingly. Do not create multiple issues for the same task. If you dont see your issue, it means it has been validated and closed. Verify this by setting the sort settings to show closed issues.

Continue with the next task to earn levels and climb the leaderboard to earn your share of the rewards!

## Recommended Reading 
[Docker - What is a Container?](https://www.docker.com/resources/what-container/)
[Alchemy Docs](https://docs.alchemy.com/)

## Labels
Label Awarded: "Modified Dapp"\
Sponsor: None
