## 4. Akash Deploy
Ok so we got the easy stuff out of the way, now its time to take your skills up a notch! If you are familiar with cloud computing, you probably know all about the enterprise services provided by Google, AWS, IBM, Oracle, etc. These services are great but are quite costly, so for the new or aspiring user their offerings may be too much. This is where [Akash Network](https://akash.network/) comes into play. Akash is a decentralized, distributed cloud provider where you pay for discreet compute services using tokens. We will be using this service to deploy a single micro-service from the RAIR suite so you can get used to how Akash works. The best part is making a simple deployment on Akash is totally free! 

## Background
In cloud computing, deployment refers to the process of making an application, service, or infrastructure available in a cloud environment. The RAIR dApp utilizes a micro-services archetecture comprised of 6 separate services which are deployed in a cluster formation and seamlessely interact with each other to create the full environment. These services are as followed:

1. RAIR-node - The central component which links and utilizes all the other services.
2. RAIR-front - The frontend component which is what you see when you access the app through your browser.
3. RAIR-sync - The synchronization engine which manages communication with the blockchain.
4. RAIR-redis - For session management.
5. RAIR-stream - The media component which manages our custom Web3 streaming service.
6. RAIR-DB - Mongo database.

In this task we will be deploying the "RAIR-front" service only.

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
11. Now click "Create Deployment".
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/15.png" width="25%"/>
12. Verify the deployment.
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/16.png" width="50%"/>
13. Wait for a bid to become available.
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/17.png" width="75%"/>
14. On the far right of your bid, click the "Select" radio button.
    <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/18.png" width="25%"/>
15. Click "Accept Bid"
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/19.png" width="25%"/>
16. The deployment will attempt to run. In this case it will fail because we are not using the full production environment but thats ok! 
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/20.png" width="75%"/>
17. Click "Leases"
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/21.png" width="25%"/>
18. Locate the "URI" and copy this link to your clipboard. If you click it, you'll see an error but for now all we need is the URI.
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/22.png" width="50%"/>
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/23.png" width="50%"/>
19. Head back to GitHub and navigate to the [Issues](https://github.com/rairprotocol/dev-dapp-season1/issues) tab in the dev-dapp-season1 repository.


20. Click "New Issue" (the green button).
21. Add a title to your issue. In this case your title should read "4. Akash Deploy".
22. Copy-paste the text below in the body of your new issue, and edit it according to our requests.
```
I deployed on Akash! My URI is [Paste URI here].
```
23. Click "Create" (the green button)

Upon completion, your task will be validated and if it is correct, you will be assigned the "Akash Deployed" label. If there is an issue, you will see the "Unresolved" label, this means there is a problem that needs to be corrected. Edit your issue and follow the guidelines more closely until you receive your "Akash Deployed" label. Do not create multiple issues for the same task. If you dont see your issue, it means it has been validated and closed. Verify this by setting the sort settings to show closed issues.

24. After you have been verified, you can terminate your deployment since its no good when its not functional. On the navigation bar click "Deployments"
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/24.png" width="25%"/>
25. You'll see your new deployment. On the far right click "..." and then close your deployment. 
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/25.png" width="75%"/>
   
Congratulations! You now know how to deploy on Akash! This was just a taste of things to come. Continue to the next task to learn how to modify the RAIR Dapp.

## Recommended Reading 
[Akash Docs](https://akash.network/docs/)

