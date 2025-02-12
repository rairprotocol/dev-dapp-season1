## 6. Modify Dapp
The ultimate goal of this season is for you to deploy your own working Dapp by utilizing our Open-Source RAIR application. RAIR comes pre-built with a ton of cool features including EVM support, custom Smart Contracts, NFT minting and marketplace capabilities, Streaming video with built-in NFT DRM protection, and more! We have designed DevDapp to help you learn and understand how to get your own Dapp up and running as easily as possible so you can focus on making something unique, without having to do all the heavy lifting. Don't let that discourage you from going nuts though. Because we are Open-Source, you can modify the code in any way you like. The sky is the limit!

This task will teach you how to get your own RAIR deployment running on localhost(your machine). You'll learn how to clone the RAIR source code, modify the environment variables to change the RPC provider, build and deploy RAIR locally using Docker, and finally you'll see it all in action in your browser. 

## Pre-Configuration
### Docker
RAIR is made up of multiple micro-services which are functionally separated from each other but which communicate together to create the full deployment. We use Docker to build the source code into "Containers", which you can think of as a single unit of software which contains all the code, dependencies, etc needed for that unit to function between different systems. You'll need to install Docker-Compose which is included with Docker-Desktop which you can get for free [here](https://www.docker.com/products/docker-desktop/). 

### Alchemy
Once you have Docker installed you'll next need a free Alchemy account to have access to your own RPC node. RPC nodes allow communication between a Blockchain and the internet since they rely on different protocols to work. Alchemy provides a limited, but free RPC node for new users so we are going to use this node in this task. Head over to [Alchemy](https://alchemy.com) and sign up to get access to the dashboard. Once in the dashboard:
1. Locate "Apps" in the sidebar.
2. Create a new app.
3. Choose "Ethereum" as your chain.
4. Activate the "Node API" service.
5. You will be directed to your new app. On the top right of the page you'll see your API key. You'll need this later.

### VSCode
If you already have a development environment of your own you can skip this step, but for those who dont you're gonna want to install an IDE(Integrated development environment) on your machine. IDEs are super helpful when working on large projects. They help you keep organized and provide a lot of functionality that will help in writing code easier. We recommend [VSCode](https://code.visualstudio.com/).

### Clone RAIR
Last but not least, you need the RAIR source code. Head to the [RAIR-Dapp](https://github.com/rairprotocol/rair-dapp) repository and download the code. There are many ways to do this but for the sake of simplicity we're just going to download the zip file to our machine, but you can also use git if you prefer. Once you have downloaded you can extract it to a location of your choice (preferably not the download directory). In your IDE, open the folder ```RAIR-Dapp-Main``` wherever you extracted it and youll see all the files. 

## Steps
We first need to configure the deployment to use your new alchemy account. We will do this by creating a ```.env``` file which contains all the variables the app might need to access before deployment. These values are referenced from this file throughout the app so they dont have to be hard-coded into the source. 
1. Locate the file in the ```Rair-Dapp-Main``` folder called ```.env.sample```
2. Make a copy of this file called ```.env```
3. Open ```.env``` and locate ```alchemy_api_key=```
4. Paste your API key from the alchemy dashboard into ```alchemy_api_key=```
Next you need to set up your RPC node. We'll use the one Alchemy gives you with your account. 
5. On the dashboard, click on "Networks"
6. Your Ethereum node should be listed at the top. Click copy to get the address.
7. In your ```.env``` locate ```ethereum_mainnet_rpc=``` and paste in the address you just copied.
8. Save your file.
9. Open a terminal in VSCode. ```terminal>new terminal``` and from the repository root enter ```docker compose -f docker-compose.local-new.yml up -d```
10. Wait for the deployment to build. (This can take several minutes)
11. Navigate to the [Issues](https://github.com/rairprotocol/dev-dapp-season1/issues) tab in the dev-dapp-season1 repository
12. Click "New Issue" (the green button).
13. Add a title to your issue. In this case your title should read "1. Github Tutorial"
14. Read first, then copy-paste the text below in the body of your new issue.

```

```
5. Click "Create" (the green button)

Upon completion, your task will be validated and if it is correct, you will be assigned the "Entered" label. If there is an issue, you will see the "Unresolved" label, this means there is a problem that needs to be corrected. Edit your issue and follow the guidelines more closely until you receive your "Entered" label. Do not create multiple issues for the same task. If you dont see your issue, it means it has been validated and closed. Verify this by setting the sort settings to show closed issues.

Congratulations! You have just created your first issue and are officially entered into DevDapp. Continue with the next task to earn levels and climb the leaderboard to earn your share of the rewards!

## Recommended Reading 
[Docker - What is a Container?](https://www.docker.com/resources/what-container/)

