[![Banner](https://github.com/rairprotocol/dev-dapp-s1/blob/main/devdapp-assets/devdapp.png)](https://devdapp.com)
[![RAIRmarket](https://img.shields.io/badge/RAIR-market-C67FD1)](https://rair.market)
[![RAIRprotocol](https://img.shields.io/badge/RAIR-protocol-C67FD1)](https://rairprotocol.org)
![License](https://img.shields.io/badge/License-Apache2.0-yellow)
[![Discord](https://img.shields.io/badge/Discord-4950AF)]([https://discord.gg/vuBUfB7w](https://discord.gg/nxVB2M4rWq))
[![Twitter](https://img.shields.io/twitter/follow/rairprotocol)](https://twitter.com/rairprotocol)

# DevDapp Season 1

Welcome to DevDapp! The GitHub Incentives Layer built on RAIRprotocol. With DevDapp you can earn tokens for contributing to our open-source! Connect your GitHub. Track Contributions. Earn RAIR + partner tokens. 

# How DevDapp Works

1. **Log in with GitHub:** Pop over to DevDapp.com and sign in with your GitHub account. This sets up your profile and tracks your progress.
3. **Complete your first task:** Watch how-to videos in the tasks section on DevDapp. 
4. **Submit your work:** Create a GitHub issue with your proof of completion (the tutorial will show you how).
5. **Get verified and earn:** If it’s all good, you’ll earn a completion label, and your profile will level up!

# Rewards

Season 1 rewards are 50,000,000 RAIR + bonus partner tokens!! Season 1 starts now. Join early to have more time to complete tasks.

# Help

If you're having trouble [Season 1 Tasks](https://github.com/rairprotocol/dev-dapp-season1/tree/main/Season%201%20Tasks) folder has all needed info. 

# Discord 

‼️ **[Come join us on Discord! ](https://discord.gg/nxVB2M4rWq)** ‼️

Our community is where we post the important announcements first, and where you can get real-time support. 

# RAIR dApp - Comprehensive Integration Master List

## 1. Blockchain Infrastructure
*Essential blockchain connectivity and interaction technologies*

| ID  | Name                                                                 | Type    | Description                                       | Importance                                            | Environment Variables                   |
|-----|----------------------------------------------------------------------|---------|---------------------------------------------------|-------------------------------------------------------|-----------------------------------------|
| 1.1 | [Ethers.js](https://github.com/ethers-io/ethers.js)                 | Library | JavaScript library for Ethereum blockchain operations | Core technology for contract calls, transactions, and wallet integration | N/A (Library)                           |
| 1.2 | [Alchemy SDK](https://auth.alchemy.com/signup)                      | SDK     | Enhanced API access to multiple blockchain networks | Provides reliable RPC capabilities and advanced blockchain data access | `ALCHEMY_API_KEY`                       |
| 1.3 | [Wagmi](https://github.com/wagmi-dev/wagmi)                         | Hooks   | React hooks library for Ethereum                 | Simplifies blockchain state management in the frontend UI | N/A (Library)                           |
| 1.4 | [Viem](https://github.com/wagmi-dev/viem)                           | Library | TypeScript interface for Ethereum interactions   | Alternative to Ethers.js for blockchain operations   | N/A (Library)                           |
| 1.5 | [Web3Auth](https://dashboard.web3auth.io/)                          | Auth    | Non-custodial wallet authentication             | Simplifies wallet onboarding with social logins      | *Requires project setup in Web3Auth dashboard* |
| 1.6 | [Account Abstraction](https://auth.alchemy.com/signup)              | SDK     | Advanced wallet features by Alchemy             | Enables gasless transactions and smart contract wallets | Uses `ALCHEMY_API_KEY`                  |
| 1.7 | [@metamask/providers](https://github.com/MetaMask/providers)        | Library | MetaMask integration                            | Connects dApp to MetaMask wallet                    | N/A (Library)                           |
| 1.8 | [@walletconnect/sign-client](https://cloud.walletconnect.com/sign-in) | Protocol | Multi-wallet connector                         | Provides broader wallet compatibility beyond MetaMask | *Requires WalletConnect project ID*     |
| 1.9 | [@metamask/onboarding](https://github.com/MetaMask/metamask-onboarding) | Library | Guides users to install MetaMask               | Assists users in wallet setup                       | N/A (Library)                           |

## 2. Storage Solutions
*Data storage across centralized and decentralized systems*

| ID  | Name                                                  | Type         | Description                              | Importance                                           | Environment Variables                              |
|-----|-------------------------------------------------------|--------------|------------------------------------------|-----------------------------------------------------|----------------------------------------------------|
| 2.1 | [MongoDB](https://www.mongodb.com/try)               | Database     | Primary persistent data store           | Stores user data, NFT metadata, and application state | `MONGO_URI`, `MONGO_URI_LOCAL`, `MONGO_DB_HOSTNAME`, `MONGO_DB_NAME` |
| 2.2 | [Redis](https://github.com/redis/redis)              | Cache        | In-memory data store                    | Handles session management and performance caching  | `REDIS_HOST`, `REDIS_PORT`                        |
| 2.3 | [IPFS](https://github.com/ipfs/ipfs)                 | Decentralized | Content-addressed storage              | Stores NFT media and provides decentralized file access | `IPFS_SERVICE`, `IPFS_GATEWAY`, `IPFS_API`         |
| 2.4 | [Pinata](https://app.pinata.cloud/register)          | Service      | IPFS pinning service                   | Ensures IPFS content availability and persistence  | `PINATA_KEY`, `PINATA_SECRET`, `PINATA_GATEWAY`   |
| 2.5 | [GCP Storage](https://cloud.google.com/free)         | Cloud        | Google Cloud Storage                   | Stores media files, backups, and centralized content | `GCP_PROJECT_ID`, `GCP_IMAGE_BUCKET_NAME`, `GCP_VIDEO_BUCKET_NAME`, `GCP_GATEWAY`, `GCP_CREDENTIALS` |
| 2.6 | [AWS S3](https://aws.amazon.com/free/)               | Cloud        | Amazon S3 object storage               | Alternative file storage and backup solution       | `AWS_ACCESS_KEY_ID`, `AWS_SECRET_ACCESS_KEY`      |
| 2.7 | [Filebase](https://filebase.com/register)            | Service      | S3-compatible decentralized storage    | Additional decentralized storage option            | `FILEBASE_ACCESS_KEY`, `FILEBASE_SECRET_ACCESS_KEY`, `FILEBASE_BUCKET` |

## 3. Backend Services
*Server-side components and utilities*

| ID   | Name                                                  | Type        | Description                             | Importance                                       | Environment Variables                  |
|------|-------------------------------------------------------|-------------|-----------------------------------------|-------------------------------------------------|----------------------------------------|
| 3.1  | [Express](https://github.com/expressjs/express)      | Framework   | Web server and API framework           | Provides API endpoints, routing, and middleware infrastructure | N/A (Framework)                        |
| 3.2  | [Mongoose](https://github.com/Automattic/mongoose)   | ODM         | MongoDB object modeling                | Handles database schema, validation, and operations | Uses MongoDB variables                 |
| 3.3  | [Socket.IO](https://github.com/socketio/socket.io)   | Realtime    | WebSocket communication                | Enables live updates, notifications, and event handling | N/A (Library)                          |
| 3.4  | [Agenda](https://github.com/agenda/agenda)           | Scheduler   | Job scheduling for Node.js             | Manages background tasks and blockchain synchronization | `SYNC_CONTRACT_REPEAT_EVERY`, `SYNC_CONTRACT_TASK_INTERVAL` |
| 3.5  | [Winston](https://github.com/winstonjs/winston)      | Logging     | Structured logging utility            | Provides application logging and monitoring    | `LOG_LEVEL`, `MONGO_LOG_COLLECTION`   |
| 3.6  | [Morgan](https://github.com/expressjs/morgan)        | Middleware  | HTTP request logger                    | Tracks API requests for debugging              | N/A (Middleware)                      |
| 3.7  | [Multer](https://github.com/expressjs/multer)        | Middleware  | File upload handling                   | Processes user-uploaded files                  | N/A (Middleware)                      |
| 3.8  | [Body Parser](https://github.com/expressjs/body-parser) | Middleware | Request body parsing                  | Handles JSON and form data in requests         | N/A (Middleware)                      |
| 3.9  | [Swagger](https://github.com/swagger-api/swagger-ui) | Documentation | API documentation                    | Provides interactive API documentation         | N/A (Documentation)                   |
| 3.10 | [Node-fetch](https://github.com/node-fetch/node-fetch) | Utility    | Server-side HTTP requests             | Facilitates API calls from backend services    | N/A (Utility)                         |
| 3.11 | [Cors](https://github.com/expressjs/cors)            | Middleware  | Cross-origin resource sharing         | Enables frontend/backend communication         | N/A (Middleware)                      |
| 3.12 | [Nanoid](https://github.com/ai/nanoid)               | Utility     | ID generation                         | Creates unique identifiers for records         | N/A (Utility)                         |
| 3.13 | [Axios](https://github.com/axios/axios)              | HTTP Client | Promise-based HTTP client             | Alternative for making API requests            | N/A (Library)                         |
| 3.14 | [Lodash](https://github.com/lodash/lodash)           | Utility     | JavaScript utility library            | Simplifies data manipulation and operations    | N/A (Utility)                         |

## 4. Frontend Framework
*User interface foundation*

| ID   | Name                                                  | Type        | Description                           | Importance                                  | Environment Variables          |
|------|-------------------------------------------------------|-------------|---------------------------------------|--------------------------------------------|-------------------------------|
| 4.1  | [React](https://github.com/facebook/react)           | Framework   | UI component library                 | Core frontend framework                   | N/A (Framework)               |
| 4.2  | [Redux Toolkit](https://github.com/reduxjs/redux-toolkit) | State      | Global state management             | Manages application state and data flow   | N/A (Library)                 |
| 4.3  | [React Router](https://github.com/remix-run/react-router) | Navigation | Client-side routing                 | Handles page transitions and navigation   | N/A (Library)                 |
| 4.4  | [Vite](https://github.com/vitejs/vite)               | Build       | Development server and bundler       | Provides fast development and optimized builds | Frontend env vars prefixed with `VITE_` |
| 4.5  | [TypeScript](https://github.com/microsoft/TypeScript) | Language   | Typed JavaScript                    | Ensures type safety and improved developer experience | N/A (Language)                |
| 4.6  | [Styled Components](https://github.com/styled-components/styled-components) | CSS | Component-level styling             | Enables modular, maintainable UI styling  | N/A (Library)                 |
| 4.7  | [MUI Material](https://github.com/mui/material-ui)   | Components  | React UI component library           | Offers pre-designed UI elements          | N/A (Library)                 |
| 4.8  | [Bootstrap](https://github.com/twbs/bootstrap)       | CSS         | Responsive design framework          | Facilitates layout and responsive design  | N/A (Library)                 |
| 4.9  | [Zustand](https://github.com/pmndrs/zustand)         | State       | Lightweight state management         | Alternative to Redux for simpler state needs | N/A (Library)                 |
| 4.10 | [React Hook Form](https://github.com/react-hook-form/react-hook-form) | Forms | Form management in React             | Simplifies form handling and validation   | N/A (Library)                 |

## 5. Media & Content Components
*Rich media handling and display*

| ID   | Name                                                  | Type        | Description                           | Importance                                  | Environment Variables |
|------|-------------------------------------------------------|-------------|---------------------------------------|--------------------------------------------|-----------------------|
| 5.1  | [Video.js](https://github.com/videojs/video.js)      | Player      | Video playback library               | Core for NFT video content playback       | N/A (Library)         |
| 5.2  | [React Player](https://github.com/cookpete/react-player) | Component | Media player component               | Provides flexible media embed options     | N/A (Component)       |
| 5.3  | [React Dropzone](https://github.com/react-dropzone/react-dropzone) | Upload | File upload UI                      | Enables drag-and-drop file uploads        | N/A (Component)       |
| 5.4  | [React Webcam](https://github.com/mozmorris/react-webcam) | Media    | Camera access component             | Facilitates live video capture            | N/A (Component)       |
| 5.5  | [React Multi Carousel](https://github.com/YIZHUANG/react-multi-carousel) | UI | Content carousel                   | Showcases multiple items in scrollable format | N/A (Component)       |
| 5.6  | [React Modal](https://github.com/reactjs/react-modal) | UI        | Dialog windows                      | Handles user interactions and confirmations | N/A (Component)       |
| 5.7  | [React Slick](https://github.com/akiran/react-slick) | UI         | Carousel alternative                | Additional option for content display     | N/A (Component)       |
| 5.8  | [React Tabs](https://github.com/reactjs/react-tabs)  | UI         | Tabbed interfaces                   | Organizes content in accessible tabs      | N/A (Component)       |
| 5.9  | [React Share](https://github.com/nygardk/react-share) | Social    | Social sharing buttons              | Enables content sharing on social platforms | N/A (Component)       |
| 5.10 | [Reactjs Popup](https://github.com/yjose/reactjs-popup) | UI       | Simple popup component              | Lightweight alternative for user feedback | N/A (Component)       |
| 5.11 | [React Hot Toast](https://github.com/timolins/react-hot-toast) | UI    | Toast notifications                 | Provides unobtrusive user notifications   | N/A (Component)       |

## 6. Security & Authentication
*Application protection and access control*

| ID   | Name                                                  | Type        | Description                           | Importance                                  | Environment Variables            |
|------|-------------------------------------------------------|-------------|---------------------------------------|--------------------------------------------|-------------------------------|
| 6.1  | [JWT](https://github.com/auth0/node-jsonwebtoken)    | Auth        | JSON Web Token authentication        | Secures API access with token-based auth  | `JWT_SECRET`                   |
| 6.2  | [Express Session](https://github.com/expressjs/session) | Session  | User session management             | Maintains persistent user sessions        | `SESSION_SECRET`, `SESSION_TTL` |
| 6.3  | [Lusca](https://github.com/krakenjs/lusca)           | Security    | Web vulnerability protection         | Guards against CSRF and XSS attacks       | N/A (Middleware)              |
| 6.4  | [Yoti](https://www.yoti.com/developers/sign-up/)     | Identity    | Identity verification                | Provides enhanced user identity verification | `YOTI_CLIENT_ID`              |
| 6.5  | [Rate Limit](https://github.com/expressjs/rate-limit) | Middleware | Request throttling                  | Prevents API abuse and DoS attacks        | `RATE_LIMIT_MINUTE`           |
| 6.6  | [CORS](https://github.com/expressjs/cors)            | Middleware  | Cross-origin resource sharing       | Controls cross-domain access to APIs      | N/A (Middleware)              |
| 6.7  | [Cookie Parser](https://github.com/expressjs/cookie-parser) | Middleware | Cookie handling              | Processes cookies for auth and preferences | N/A (Middleware)              |
| 6.8  | [Connect-Redis](https://github.com/visionmedia/connect-redis) | Session | Redis session store                | Integrates Redis with Express sessions    | Uses Redis variables          |

## 7. Wallet Integration
*Blockchain wallet connectivity*

| ID   | Name                                                  | Type        | Description                           | Importance                                  | Environment Variables          |
|------|-------------------------------------------------------|-------------|---------------------------------------|--------------------------------------------|-------------------------------|
| 7.1  | [MetaMask](https://github.com/MetaMask/metamask-extension) | Wallet | Browser extension wallet            | Primary user wallet connection method     | N/A (Client-side)             |
| 7.2  | [WalletConnect](https://cloud.walletconnect.com/sign-in) | Protocol | Multi-wallet connector              | Enables broader wallet compatibility      | *Requires WalletConnect project ID* |
| 7.3  | [Web3Auth](https://dashboard.web3auth.io/)            | Auth        | Social login for wallets             | Simplifies wallet authentication experience | *Requires Web3Auth credentials* |
| 7.4  | [Alchemy AA](https://auth.alchemy.com/signup)         | SDK         | Account abstraction                  | Enables smart contract wallets and advanced features | Uses `ALCHEMY_API_KEY`        |

## 8. Development & DevOps
*Development workflow and quality tools*

| ID   | Name                                                  | Type        | Description                           | Importance                                  | Environment Variables                              |
|------|-------------------------------------------------------|-------------|---------------------------------------|--------------------------------------------|-------------------------------------------|
| 8.1  | [ESLint](https://github.com/eslint/eslint)           | Linter      | Code quality enforcement             | Maintains code standards and prevents errors | N/A (Dev tool)                            |
| 8.2  | [Prettier](https://github.com/prettier/prettier)     | Formatter   | Code formatting                      | Ensures consistent code style             | N/A (Dev tool)                            |
| 8.3  | [Husky](https://github.com/typicode/husky)           | Git Hooks   | Pre-commit tasks                     | Automates code quality checks             | N/A (Dev tool)                            |
| 8.4  | [Nodemon](https://github.com/remy/nodemon)           | Dev         | Server auto-restart                  | Improves development workflow efficiency  | N/A (Dev tool)                            |
| 8.5  | [Docker](https://github.com/docker/docker-ce)        | Container   | Application containerization         | Ensures deployment and environment consistency | N/A (Infrastructure)                     |
| 8.6  | [Vault](https://www.vaultproject.io/downloads)       | Security    | Secret management                    | Securely manages application credentials  | `VAULT_URL`, `VAULT_*_APP_ROLE_ID`, `VAULT_*_APP_ROLE_SECRET_ID` |
| 8.7  | [Dotenv](https://github.com/motdotla/dotenv)         | Config      | Environment variables                | Manages configuration across environments | N/A (Dev tool)                            |

## 9. Monitoring & Analytics
*Application health and user insights*

| ID   | Name                                                  | Type        | Description                           | Importance                                  | Environment Variables                              |
|------|-------------------------------------------------------|-------------|---------------------------------------|--------------------------------------------|-------------------------------------------|
| 9.1  | [Sentry](https://sentry.io/signup/)                  | Monitoring  | Error tracking                       | Ensures application reliability and issue detection | `SENTRY_DSN`, `VITE_SENTRY_ENABLED`, `VITE_SENTRY_IO_ENDPOINT`, `VITE_SENTRY_IO_TRACE_RATE`, `VITE_SENTRY_RELEASE` |
| 9.2  | [Google Analytics](https://analytics.google.com/)    | Analytics   | Usage metrics                        | Tracks user behavior and interactions     | `VITE_GOOGLE_ANALYTICS`, `VITE_GA_NAME`   |
| 9.3  | [Custom Events](https://github.com/)                 | Tracking    | Event monitoring                     | Provides flexible interaction tracking    | N/A (Implementation-specific)             |
| 9.4  | [React GA](https://github.com/react-ga/react-ga)     | Analytics   | Google Analytics for React           | Integrates GA specifically with React     | Uses Google Analytics variables           |

*Note: Custom Events lacks a specific GitHub repository as it’s implementation-specific; no URL is provided.*

## 10. Microservices Architecture
*Core services that compose the application*

| ID    | Name                                                  | Type        | Description                           | Importance                                  | Environment Variables          |
|-------|-------------------------------------------------------|-------------|---------------------------------------|--------------------------------------------|-------------------------------|
| 10.1  | [rairnode](https://github.com/RAIRprotocol/rairnode) | Service     | Main backend API service             | Provides primary API endpoints and business logic | Multiple (see docker-compose) |
| 10.2  | [blockchain-networks](https://github.com/)           | Service     | Blockchain data synchronization      | Syncs data from multiple blockchain networks | Multiple (see docker-compose) |
| 10.3  | [media-service](https://github.com/)                 | Service     | Media processing service             | Handles media file processing and delivery | `MEDIA_SERVICE_PORT`, `BASE_RAIRNODE_URL` + storage vars |
| 10.4  | [rair-redis](https://github.com/redis/redis)         | Service     | In-memory data store                 | Manages sessions and caching              | Redis configuration           |
| 10.5  | [minting-network](https://github.com/)               | Service     | Frontend dApp                        | User-facing application for NFT minting   | Frontend-specific variables   |

*Note: Some microservices (blockchain-networks, media-service, minting-network) lack public GitHub repositories; no URLs are provided where unavailable.*

## 11. Blockchain Networks
*Supported blockchain networks in the system*

| ID    | Name                                                  | Type        | Description                           | Importance                                  | Environment Variables                              |
|-------|-------------------------------------------------------|-------------|---------------------------------------|--------------------------------------------|-------------------------------------------|
| 11.1  | [Ethereum Mainnet](https://ethereum.org/en/developers/) | Network   | Production Ethereum network          | Primary Ethereum blockchain environment   | `ETHEREUM_MAINNET_RPC`, `ETHEREUM_MAINNET_FACTORY_ADDRESS`, `ETHEREUM_MAINNET_MINTER_ADDRESS` |
| 11.2  | [Ethereum Sepolia](https://sepolia.dev/)             | Network     | Ethereum testnet                     | Testing environment for Ethereum          | `ETHEREUM_TESTNET_SEPOLIA_RPC`, `SEPOLIA_FACTORY_ADDRESS`, `SEPOLIA_MINTER_ADDRESS`, etc. |
| 11.3  | [Polygon/Matic Mainnet](https://polygon.technology/)  | Network     | Production Polygon network           | Scalable production environment           | `MATIC_MAINNET_RPC`, `MATIC_MAINNET_FACTORY_ADDRESS`, `MATIC_MAINNET_MINTER_ADDRESS`, etc. |
| 11.4  | [Polygon/Matic Mumbai](https://mumbai.polygon.technology/) | Network | Polygon testnet                     | Testing environment for Polygon           | `MATIC_TESTNET_RPC`, `MATIC_MUMBAI_FACTORY_ADDRESS`, `MATIC_MUMBAI_MINTER_ADDRESS`, etc. |
| 11.5  | [Binance Smart Chain](https://www.bnbchain.org/en)    | Network     | Production BSC network               | Alternative production blockchain         | `BINANCE_MAINNET_RPC`, `BINANCE_MAINNET_FACTORY_ADDRESS`, `BINANCE_MAINNET_MINTER_ADDRESS`, etc. |
| 11.6  | [Binance Testnet](https://testnet.bnbchain.org/)      | Network     | BSC testnet                          | Testing environment for BSC               | `BINANCE_TESTNET_RPC`, `BINANCE_TESTNET_FACTORY_ADDRESS`, `BINANCE_TESTNET_MINTER_ADDRESS`, etc. |
| 11.7  | [Base](https://base.org/)                             | Network     | Production Base network              | Ethereum L2 scaling solution              | `BASE_MAINNET_RPC`, `BASE_DIAMOND_FACTORY_ADDRESS`, `BASE_DIAMOND_MARKETPLACE_ADDRESS` |
| 11.8  | [Astar](https://astar.network/)                       | Network     | Production Astar network             | Polkadot parachain integration            | `ASTAR_MAINNET_RPC`, `ASTAR_DIAMOND_FACTORY_ADDRESS`, `ASTAR_DIAMOND_MARKETPLACE_ADDRESS` |

## 12. External Services
*Third-party integrations*

| ID    | Name                                                  | Type        | Description                           | Importance                                  | Environment Variables          |
|-------|-------------------------------------------------------|-------------|---------------------------------------|--------------------------------------------|-------------------------------|
| 12.1  | [Alchemy](https://auth.alchemy.com/signup)            | Blockchain  | Enhanced RPC provider                | Provides reliable blockchain connectivity | `ALCHEMY_API_KEY`             |
| 12.2  | [Pinata](https://app.pinata.cloud/register)           | Storage     | IPFS pinning service                 | Ensures decentralized content persistence | `PINATA_KEY`, `PINATA_SECRET`, `PINATA_GATEWAY` |
| 12.3  | [Google Cloud Platform](https://cloud.google.com/free) | Cloud      | Cloud services provider              | Hosts various infrastructure components   | `GCP_PROJECT_ID`, `GCP_CREDENTIALS`, etc. |
| 12.4  | [Sentry.io](https://sentry.io/signup/)                | Monitoring  | Error tracking service               | Tracks application errors and performance | `SENTRY_DSN`                  |
| 12.5  | [Zoom](https://zoom.us/signup)                        | Communication | Video meetings integration          | Facilitates video communication features  | `ZOOM_API_KEY`, `ZOOM_API_SECRET`, `ZOOM_MEETING_ID` |
| 12.6  | [Yoti](https://www.yoti.com/developers/sign-up/)      | Identity    | ID verification service              | Provides KYC and identity verification    | `YOTI_CLIENT_ID`              |


# RAIRprotocol Master API List 

---

## Authentication
Endpoints related to user authentication, including wallet sign-in and session management.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/auth/get_challenge`          | POST   | Generate challenge for wallet sign-in| None           | Initiates web3 authentication flow |
| `/auth/login`                  | POST   | Login with wallet signature          | None           | Core authentication endpoint    |
| `/auth/loginSmartAccount`      | POST   | Login with smart account signature   | None           | Support for smart contract wallets |
| `/auth/logout`                 | GET    | Logout user session                  | User Session   | Session management             |
| `/auth/me`                     | GET    | Get current user details             | User Session   | Session verification           |
| `/auth/unlock`                 | POST   | Unlock media with session            | User Session   | Content access management      |
| `/auth/stream/out`             | GET    | End media stream authorization       | User Session   | Media streaming control        |

---

## User Management
Endpoints for managing user profiles and related administrative tasks.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/users/list`                  | GET    | List all users                       | Admin          | User management for admins      |
| `/users/export`                | GET    | Export users as CSV                  | Admin          | Data export functionality       |
| `/users/verify-age`            | POST   | Verify user age with Yoti            | User Session   | Age verification compliance     |
| `/users/:publicAddress`        | GET    | Get user by wallet address           | None           | Public profile retrieval        |
| `/users/:publicAddress`        | PATCH  | Update user profile                  | User Session   | Profile management             |

---

## NFT Management
Endpoints for creating, retrieving, and managing non-fungible tokens (NFTs).

| Endpoint                                              | Method | Description                          | Authentication | Importance                      |
|-------------------------------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/nft`                                                | POST   | Create tokens via CSV                | Admin          | Bulk token creation             |
| `/nft`                                                | GET    | Get current user's tokens            | User Session   | Token discovery                 |
| `/nft/:userAddress`                                   | GET    | Get tokens by user address           | None           | Profile token view              |
| `/nft/csv/sample`                                     | GET    | Get metadata CSV sample              | None           | Help for token creation         |
| `/nft/pinningMultiple`                                | POST   | Pin multiple token metadata to IPFS  | User Session   | Token metadata persistence      |
| `/nft/network/:networkId/:contract/:product`          | GET    | Get tokens for product               | None           | Token discovery                 |
| `/nft/network/:networkId/:contract/:product/numbers`  | GET    | Get token numbers                    | None           | Token ID enumeration            |
| `/nft/network/:networkId/:contract/:product/attributes` | GET  | Get product attributes               | None           | Metadata attribute discovery    |
| `/nft/network/:networkId/:contract/:product/files`    | GET    | Get files for product                | None           | Product content discovery       |
| `/nft/network/:networkId/:contract/:product/files/:token` | GET | Get files for token                 | None           | Token content discovery         |
| `/nft/network/:networkId/:contract/:product/offers`   | GET    | Get offers for product               | None           | Product offer discovery         |
| `/nft/network/:networkId/:contract/:product/locks`    | GET    | Get locked offers for product        | None           | Locked offer discovery          |
| `/nft/network/:networkId/:contract/:product/token/:token` | GET | Get single token                    | None           | Detailed token info             |
| `/nft/network/:networkId/:contract/:product/token/:token` | POST | Update token metadata              | User Session   | Metadata management             |
| `/nft/network/:networkId/:contract/:product/token/:token/pinning` | POST | Pin single token metadata       | User Session   | IPFS persistence                |

---

## Tokens
Endpoints for retrieving information about tokens (potentially including both fungible and non-fungible tokens).

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/tokens`                      | GET    | Get all tokens                       | None           | Token discovery                 |
| `/tokens/:token`               | GET    | Get token by number                  | None           | Token lookup                    |
| `/tokens/id/:id`               | GET    | Get token by ID                      | None           | Token lookup by database ID     |

---

## Contract Management
Endpoints for managing smart contracts and their associated data.

| Endpoint                                      | Method | Description                          | Authentication      | Importance                      |
|-----------------------------------------------|--------|--------------------------------------|---------------------|---------------------------------|
| `/contracts`                                  | GET    | Get all contracts                    | None                | Contract discovery              |
| `/contracts/factoryList`                      | GET    | Get contracts for factory            | User Session        | Factory contract discovery      |
| `/contracts/my`                               | GET    | Get user's contracts                 | User Session        | User's contract discovery       |
| `/contracts/full`                             | GET    | Get full contract list               | None                | Enhanced contract discovery     |
| `/contracts/network/:networkId/:contractAddress` | GET  | Find contract by network and address | None                | Contract lookup                 |
| `/contracts/network/:networkId/:contractAddress/products` | GET | Get products for contract         | None                | Contract product discovery      |
| `/contracts/network/:networkId/:contractAddress/offers` | GET | Get offers for contract           | None                | Contract offer discovery        |
| `/contracts/import`                           | POST   | Import external contract             | Admin + Super Admin | Contract importing              |
| `/contracts/:id`                              | GET    | Get contract by ID                   | None                | Contract details                |
| `/contracts/:id`                              | PATCH  | Update contract                      | Admin + Super Admin | Contract management             |

---

## File Management
Endpoints for managing media files and their metadata.

| Endpoint                       | Method | Description                          | Authentication      | Importance                      |
|--------------------------------|--------|--------------------------------------|---------------------|---------------------------------|
| `/files/update/:mediaId`       | PATCH  | Update media file                    | User Session + Owner| Content management              |
| `/files/remove/:mediaId`       | DELETE | Delete media file                    | User Session + Owner| Content deletion                |
| `/files/list`                  | GET    | List media files                     | None                | Content discovery               |
| `/files/byId/:id`              | GET    | Get file by ID                       | None                | File lookup                     |
| `/files/byId/:id`              | PUT    | Update file                          | User Session + Owner| File management                 |
| `/files/byCategory/:id`        | GET    | Get files by category                | None                | Category-based discovery        |
| `/files/forToken/:id`          | GET    | Get files for token                  | None                | Token file lookup               |
| `/files/categories`            | GET    | List file categories                 | None                | Category discovery              |
| `/files/:id/unlocks`           | GET    | Get file unlock offers               | None                | File access management          |
| `/files/:id/unlocks`           | POST   | Create file unlock offer             | User Session + Owner| File access management          |
| `/files/:id/unlocks`           | DELETE | Remove file unlock offer             | User Session + Owner| File access management          |

---

## Transactions
Endpoints for processing user transactions.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/transactions/:network/:hash` | POST   | Process user transaction             | User Session   | Transaction recording and processing |

---

## Product Management
Endpoints for managing products within the platform.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/products`                    | GET    | Get all products                     | None           | Product discovery               |
| `/products/user/:userAddress`  | GET    | Get products by user                 | None           | User-specific products          |
| `/products/:id`                | GET    | Get product by ID                    | None           | Product lookup                  |
| `/products/:id`                | POST   | Set product banner                   | None           | Product customization           |

---

## Credits and Payments
Endpoints for managing user credits and withdrawals.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/credits/:blockchain/:tokenAddress` | GET  | Get user credits                    | User Session   | Balance checking                |
| `/credits/withdraw`            | POST   | Generate withdraw request            | User Session   | Fund withdrawal                 |

---

## Settings & Configuration
Endpoints for managing server and application settings.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/settings`                    | GET    | Get server settings                  | None           | System configuration            |
| `/settings/blockchain`         | POST   | Set blockchain setting               | Super Admin    | Blockchain configuration        |
| `/settings/appLogo`            | POST   | Set application logo                 | Admin          | Branding                        |
| `/settings/theme`              | GET    | Get theme settings                   | None           | UI customization                |
| `/settings/featured-collection`| GET    | Get featured collection              | None           | Homepage featured content       |

---

## Analytics & Reports
Endpoints for retrieving analytics data and reports.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/analytics/:mediaId`          | GET    | Get analytics data                   | User Session   | Performance tracking            |
| `/analytics/:mediaId/csv`      | GET    | Get analytics CSV report             | User Session   | Data export                     |

---

## Search
Endpoints for performing searches across the platform.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/search/:textParam`           | GET    | Global search                        | None           | Content discovery               |
| `/search/:textParam/all`       | GET    | Expanded global search               | None           | Enhanced discovery              |

---

## Notifications
Endpoints for managing user notifications.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/notifications`               | GET    | List notifications                   | User Session   | User notifications              |
| `/notifications/:id`           | GET    | Get single notification              | User Session   | Notification details            |
| `/notifications`               | PUT    | Mark notifications as read           | User Session   | Notification management         |
| `/notifications`               | DELETE | Delete notifications                 | User Session   | Notification management         |

---

## Favorites
Endpoints for managing user favorites.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/favorites`                   | POST   | Create favorite                      | User Session   | User preferences                |
| `/favorites`                   | GET    | Get user favorites                   | User Session   | User saved items                |
| `/favorites/:address`          | GET    | Get favorites of address             | None           | Public favorites                |
| `/favorites/:id`               | DELETE | Delete favorite                      | User Session   | Favorite management             |

---

## Categories
Endpoints for managing content categories.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/categories`                  | GET    | Get categories                       | None           | Content organization            |
| `/categories`                  | POST   | Update categories                    | Super Admin    | Category management             |

---

## Uploads
Endpoints for uploading and validating files.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/upload/validate`             | GET    | Validate media data                  | None           | Content validation              |
| `/upload`                      | POST   | Upload file                          | None           | File upload                     |
| `/upload/token`                | GET    | Get upload token                     | None           | Upload authorization            |

---

## Resales & Secondary Market
Endpoints for managing resale offers and secondary market transactions.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/resales/open`                | GET    | Get open resales                     | None           | Secondary market discovery      |
| `/resales/create`              | POST   | Create resale offer                  | User Session   | Secondary market listing        |
| `/resales/:id`                 | PATCH  | Update resale offer                  | User Session   | Offer management                |
| `/resales/:id`                 | DELETE | Delete resale offer                  | User Session   | Offer removal                   |
| `/resales/:id/purchase`        | POST   | Generate purchase request            | User Session   | Secondary market purchase       |

---

## Offers
Endpoints for managing offers across the platform.

| Endpoint                       | Method | Description                          | Authentication | Importance                      |
|--------------------------------|--------|--------------------------------------|----------------|---------------------------------|
| `/offers`                      | GET    | Get all offers                       | None           | Offer discovery                 |
| `/offers/:id`                  | PATCH  | Update offer data                    | Admin          | Offer management                |

---
