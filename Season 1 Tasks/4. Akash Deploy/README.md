## 4. Akash Deploy
Ok so we got the easy stuff out of the way, now its time to take your skills up a notch! If you are familiar with cloud computing, you probably know all about the enterprise services provided by Google, AWS, IBM, Oracle, etc. These services are great but are quite costly, so for the new or aspiring user their offerings may be too much. This is where [Akash Network](https://akash.network/) comes into play. Akash is a decentralized, distributed cloud provider where you pay for compute services using tokens. We will be using this service to deploy a fully functional RAIR node which is yours to explore, modify, and extend to your hearts desire! The best part is you dont need a credit card to get going! Akash provides free tokens to get started so it wont cost you anything to complete this task! 

## Background
In cloud computing, deployment refers to the process of making an application, service, or infrastructure available in a cloud environment. The RAIR dApp utilizes a micro-services archetecture comprised of 5 separate services which are deployed in a cluster formation and seamlessely interact with each other to create the full environment. These services are as followed:

1. RAIR-node - The central component which links and utilizes all the other services.
2. RAIR-front - The frontend component which is what you see when you access the app through your browser.
3. RAIR-sync - The synchronization engine which manages communication with the blockchain.
4. RAIR-redis - For session management.
5. RAIR-stream - The media component which manages our custom Web3 streaming service.

Configuring all of these services to deploy is beyond the scope of this task but thats ok! We have preconfigured a deployment for you so getting your RAIR dApp up and running is as simple as the click of a button. Don't let this discourage you from digging in and seeing how it all works, but for now we'll do all the heavy lifting.

## Steps
1. Head to the [Akash Console](https://console.akash.network/).
2. At the top of the page click "Start Trial".\
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/01.png" width="25%"/>
3. You will receive temporary trial funds. 
  <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/02.png" width="25%"/>
4. On the left side of the page, click "Templates".
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/03.png" width="25%"/>
5. In "Filter Templates" click "Business".
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/04.png" width="25%"/>
6. Click "RAIR-Dapp".
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/05.png" width="25%"/>
7. This will take you to an info page telling you about the deployment. To the right of "RAIR-Dapp" click "Deploy".
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/06.png" width="25%"/>
8. Inside the "Create Deployment" menu, click "Builder".
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/07.png" width="25%"/>
9. Our production deployment is too big for the trial, so we need to pare it down. In this task we are just going to deploy the "RAIR-front" microservice, so locate the other services and delete them from the deployment by clicking the trash icon on the far right.
    <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/08.png" width="75%"/>
    <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/09.png" width="75%"/>
    <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/10.png" width="75%"/>
    <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/11.png" width="75%"/>
    <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/12.png" width="75%"/>
10. This leaves just the "RAIR-front" service.
    <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/14.png" width="75%"/>
5. Navigate to the [Issues](https://github.com/rairprotocol/dev-dapp-season1/issues) tab in the dev-dapp-season1 repository
6. Click "New Issue" (the green button).
7. Add a title to your issue. In this case your title should read "2. Favorite EIP"
8. Copy-paste the text below in the body of your new issue, and edit it according to our requests.
9. Click "Create" (the green button)

```
I checked out Ethereum Improvement Proposals! My Favorite new EIP is [Write EIP here].

The reason I like this EIP is [Write a short description why, this helps us understand what features we might want to implement in the future to our own smart contracts!]
```
Upon completion, your task will be validated and if it is correct, you will be assigned the "Favorite EIP" label. If there is an issue, you will see the "Unresolved" label, this means there is a problem that needs to be corrected. Edit your issue and follow the guidelines more closely until you receive your "Favorite EIP" label. Do not create multiple issues for the same task. If you dont see your issue, it means it has been validated and closed. Verify this by setting the sort settings to show closed issues.

Congratulations! Continue with the next task to earn levels and climb the leaderboard to earn your share of the rewards!

## Recommended Reading 
[Ethereum Improvement Proposals- Creating an Issue](https://eips.ethereum.org/)\
[Introduction to Smart Contracts](https://ethereum.org/en/developers/docs/smart-contracts/)
