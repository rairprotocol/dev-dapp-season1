## 4. Akash Deploy
Now that we’ve covered the basics, it's time to level up! Traditional cloud services like AWS and Google Cloud can be expensive, but [Akash Network](https://akash.network/) offers a decentralized alternative, letting you pay for compute services with tokens. In this task, you'll deploy the ```RAIR-front``` microservice on Akash—for free!

## Background
RAIR dApp uses a microservices architecture with six components:

1. **RAIR-node** - Central hub connecting all services
2. **RAIR-front** - Web frontend
3. **RAIR-sync** - Blockchain sync engine
4. **RAIR-redis** - Session management
5. **RAIR-stream** - Web3 streaming
6. **RAIR-DB** - Mongo DB.

For this task, we'll only deploy ``RAIR-front``.

## Steps
1. Head to [Akash Console](https://console.akash.network/).
2. At the top of the page click "Start Trial".\
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/01.png" width="25%"/>
3. Receive temporary trial funds. 
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
13. Wait for a bid to become available. If you dont receive a bid, its because Akash trial servers are overloaded. You may have to try again later.
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
19. Go to [Issues](https://github.com/rairprotocol/dev-dapp-season1/issues) tab.
20. Click "New Issue" (green button).
21. Title to your issue "4. Akash Deploy".
22. Paste the example issue text in the body, replacing [Paste URI here] with your copied URI:
23. Click "Create" (the green button)
24. After you have been verified, you can terminate your deployment since its no good when its not functional. On the navigation bar click "Deployments"
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/24.png" width="25%"/>
25. You'll see your new deployment. On the far right click "..." and then close your deployment. 
   <img src="https://github.com/rairprotocol/dev-dapp-season1/blob/main/devdapp-assets/Season%201%20Tasks/4.%20Akash%20Deploy/25.png" width="75%"/>

## Example Issue Body
```
I deployed on Akash! My URI is [Paste URI here].
```

## Completion
Great job! You’ve completed your first Akash deployment. You will be assigned the "Akash Deployed" label. If there is an issue, you will see the "Unresolved" label. Do not create multiple issues for the same task. If you dont see your issue, it means it has been validated and closed. Verify this by setting the sort settings to show closed issues. 
   
Up next: modifying the RAIR dApp. 

## Recommended Reading 
[Akash Docs](https://akash.network/docs/)

## Labels
Label Awarded: "Akash Deployed"\
Sponsor: "Akash"
