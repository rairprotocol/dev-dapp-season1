[![Banner](https://github.com/rairprotocol/dev-dapp-s1/blob/main/devdapp-assets/devdapp.png)](https://devdapp.com)
[![RAIRmarket](https://img.shields.io/badge/RAIR-market-C67FD1)](https://rair.market)
[![RAIRprotocol](https://img.shields.io/badge/RAIR-protocol-C67FD1)](https://rairprotocol.org)
![License](https://img.shields.io/badge/License-Apache2.0-yellow)
[![Discord](https://img.shields.io/badge/Discord-4950AF)]([https://discord.gg/vuBUfB7w](https://discord.gg/nxVB2M4rWq))
[![Twitter](https://img.shields.io/twitter/follow/rairprotocol)](https://twitter.com/rairprotocol)

# DevDapp Season 1

Welcome to DevDapp! The GitHub Incentives Layer built on RAIRprotocol. With DevDapp you can earn tokens for contributing to our open-source! Connect your GitHub. Track Contributions. Earn RAIR + partner tokens. 

# How DevDapp Works
RAIRprotocol is a Dapp building engine. By completing the initial 8 tasks in DevDapp you'll earn tokens and learn how to deploy a working Dapp! 

1. If you haven't done so yet, the first step to start playing is by logging in with your GitHub account on [DevDapp.com](Https://devdapp.com). This creates your in-game account and is necessary for tracking your progression.
2. Next, you need to select a task. Scroll down on DevDapp.com and locate the "Tasks" section. Here you can watch an introductory video for the task and you'll find a link to the GitHub tutorial to help you complete it.
![initial-tasks](https://github.com/rairprotocol/dev-dapp-s1/blob/main/devdapp-assets/initial-tasks.png)
3. Complete the task.
4. Make a new issue in the GitHub for your task. The tutorial will show you how to format your proof of completion.
5. If everything checks out, you will receive a label on your task showing you have completed the task. This will update your profile on DevDapp.com with your new levels.
6. Keep playing to earn more levels and climb the leaderboards to earn your share of the $60k prize pool. Prizes are distributed at the end of the season (May 2025).
From there the sky is the limit to build your own Dapp. Or join a team to help them build their dapps. In this first season you are automatically added to the DevDapp team by default. Teams will be expanded in later seasons.

# Rewards

Season 1 rewards are 50,000,000 RAIR + bonus partner tokens!! Season 1 starts now through May 2025. Join early to have more time to complete tasks. Your rewards will be held in an abstracted Alchemy smart wallet that is connected to your GitHub account and will be released to you at the end of the season.

# Help

If you're having trouble with a particular task, please check out the [Season 1 Tasks](https://github.com/rairprotocol/dev-dapp-season1/tree/main/Season%201%20Tasks) folder in our GitHub repository for helpful information regarding your current task.

# Comprehensive dApp Architecture & Services

## System Architecture

### Microservices
*Core services that compose the application*

| Service | Purpose | Key Integrations |
|---------|---------|------------------|
| **rairnode** | Main backend service with API endpoints | MongoDB, Redis, JWT, IPFS |
| **blockchain-networks** | Blockchain data synchronization | Agenda, Ethers.js, MongoDB |
| **media-service** | Media file processing and delivery | GCP Storage, Pinata, IPFS |
| **rair-redis** | In-memory data store | Session management, Caching |
| **minting-network** | Frontend dApp for NFT minting | React, Redux, Web3 wallets |

## Core Technologies

### 1. Blockchain Infrastructure
*Essential blockchain connectivity and interaction*

| Name | Type | Description | Usage |
|------|------|-------------|-------|
| Ethers.js | Library | Ethereum blockchain operations | Contract calls, transactions, wallet integration |
| Alchemy SDK | SDK | Blockchain data access across networks | Network access, enhanced RPC capabilities |
| Wagmi | Hooks | React hooks for Ethereum | Simplified blockchain state handling in UI |
| Viem | Library | TypeScript interface for Ethereum | Alternative blockchain interactions |
| Web3Auth | Auth | Wallet authentication | Simplified wallet onboarding |
| Account Abstraction | SDK | Advanced wallet features | Gasless transactions, account management |

### 2. Storage Solutions
*Data storage across centralized and decentralized systems*

| Name | Type | Description | Usage |
|------|------|-------------|-------|
| MongoDB | Database | Primary persistent data store | User data, NFT metadata, application state |
| Redis | Cache | In-memory data store | Session management, caching, performance |
| IPFS | Decentralized | Content-addressed storage | NFT media, decentralized file storage |
| Pinata | Service | IPFS pinning service | Ensures IPFS content availability |
| GCP Storage | Cloud | Google Cloud Storage | Media files, backups, centralized storage |
| AWS S3 | Cloud | Amazon S3 object storage | Alternative file storage, backups |
| Filebase | Service | S3-compatible decentralized storage | Additional decentralized storage option |

### 3. Backend Services
*Server-side components and utilities*

| Name | Type | Description | Usage |
|------|------|-------------|-------|
| Express | Framework | Web server and API framework | API endpoints, routing, middleware |
| Mongoose | ODM | MongoDB object modeling | Database schema, validation, operations |
| Socket.IO | Realtime | WebSocket communication | Live updates, notifications, events |
| Agenda | Scheduler | Job scheduling for Node.js | Background tasks, blockchain syncing |
| Winston | Logging | Structured logging utility | Application logging, monitoring |
| Morgan | Middleware | HTTP request logger | API request tracking, debugging |
| Multer | Middleware | File upload handling | Processing user uploaded files |
| Body Parser | Middleware | Request body parsing | Handling JSON and form data |
| Swagger | Documentation | API documentation | Interactive API documentation |

### 4. Frontend Framework
*User interface foundation*

| Name | Type | Description | Usage |
|------|------|-------------|-------|
| React | Framework | UI component library | Core frontend framework |
| Redux Toolkit | State | Global state management | Application state, data flow |
| React Router | Navigation | Client-side routing | Page transitions, navigation |
| Vite | Build | Dev server and bundler | Fast development, optimized builds |
| TypeScript | Language | Typed JavaScript | Type safety, better developer experience |
| Styled Components | CSS | Component-level styling | Modular, maintainable UI styling |
| MUI Material | Components | React UI component library | Pre-designed UI elements |
| Bootstrap | CSS | Responsive design framework | Layout, responsive design |

### 5. Media & Content Components
*Rich media handling and display*

| Name | Type | Description | Usage |
|------|------|-------------|-------|
| Video.js | Player | Video playback library | NFT video content playback |
| React Player | Component | Media player component | Flexible media embed options |
| React Dropzone | Upload | File upload UI | Drag-and-drop file uploads |
| React Webcam | Media | Camera access component | Live video capture |
| React Multi Carousel | UI | Content carousel | Showcase multiple items |
| React Modal | UI | Dialog windows | User interactions, confirmations |

### 6. Security & Authentication
*Application protection and access control*

| Name | Type | Description | Usage |
|------|------|-------------|-------|
| JWT | Auth | JSON Web Token authentication | Secure API access |
| Express Session | Session | User session management | Persistent user sessions |
| Lusca | Security | Web vulnerability protection | CSRF, XSS protection |
| Yoti | Identity | Identity verification | Enhanced identity verification |
| Rate Limit | Middleware | Request throttling | API abuse prevention |
| CORS | Middleware | Cross-origin resource sharing | Frontend/backend communication |

### 7. Wallet Integration
*Blockchain wallet connectivity*

| Name | Type | Description | Usage |
|------|------|-------------|-------|
| MetaMask | Wallet | Browser extension wallet | Primary user wallet connection |
| WalletConnect | Protocol | Multi-wallet connector | Broader wallet compatibility |
| Web3Auth | Auth | Social login for wallets | Simplified wallet authentication |
| Alchemy AA | SDK | Account abstraction | Smart contract wallets |

### 8. Development & DevOps
*Development workflow and quality tools*

| Name | Type | Description | Usage |
|------|------|-------------|-------|
| ESLint | Linter | Code quality enforcement | Code standards, error prevention |
| Prettier | Formatter | Code formatting | Consistent code style |
| Husky | Git Hooks | Pre-commit tasks | Code quality automation |
| Nodemon | Dev | Server auto-restart | Development workflow efficiency |
| Docker | Container | Application containerization | Deployment, environment consistency |
| Vault | Security | Secret management | Secure credential management |

### 9. Monitoring & Analytics
*Application health and user insights*

| Name | Type | Description | Usage |
|------|------|-------------|-------|
| Sentry | Monitoring | Error tracking | Application reliability |
| Google Analytics | Analytics | Usage metrics | User behavior tracking |
| Custom Events | Tracking | Event monitoring | Flexible interaction tracking |

## Blockchain Networks
*Supported blockchain networks in the system*

| Network | Type | RPC Variables | Related Contracts |
|---------|------|--------------|------------------|
| Ethereum Mainnet | Production | ETHEREUM_MAINNET_RPC | Diamond Marketplace, Factory |
| Ethereum Sepolia | Testnet | ETHEREUM_TESTNET_SEPOLIA_RPC | Diamond Marketplace, Factory |
| Polygon/Matic Mainnet | Production | MATIC_MAINNET_RPC | Diamond Marketplace, Factory |
| Polygon/Matic Mumbai | Testnet | MATIC_TESTNET_RPC | Diamond Marketplace, Factory |
| Binance Smart Chain | Production | BINANCE_MAINNET_RPC | Diamond Marketplace, Factory |
| Binance Testnet | Testnet | BINANCE_TESTNET_RPC | Diamond Marketplace, Factory |
| Base | Production | BASE_MAINNET_RPC | Diamond Marketplace, Factory |
| Astar | Production | ASTAR_MAINNET_RPC | Diamond Marketplace, Factory |

## External Integrations
*Third-party services integrated in the application*

| Service | Category | Purpose | Variables |
|---------|----------|---------|-----------|
| Alchemy | Blockchain | Enhanced RPC, AA | ALCHEMY_API_KEY |
| Pinata | Storage | IPFS pinning | PINATA_KEY, PINATA_SECRET |
| GCP | Cloud | Cloud storage | GCP_CREDENTIALS, GCP_PROJECT_ID |
| Sentry | Monitoring | Error tracking | SENTRY_DSN |
| Zoom | Communication | Video meetings | ZOOM_API_KEY, ZOOM_API_SECRET |
| Yoti | Identity | ID verification | YOTI_CLIENT_ID |
| Google Analytics | Analytics | Usage tracking | GOOGLE_ANALYTICS |


# Discord 

‼️ **[Come join us on Discord! ](https://discord.gg/nxVB2M4rWq)** ‼️

Our community is where we post the important announcements first, and where you can get real-time support. 
