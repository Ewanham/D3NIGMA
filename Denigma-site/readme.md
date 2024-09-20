## Installation 🛠️
Setting up your project and deploying your contract is straightforward with detailed guide:

### 1. Setting Up Your Project
- Install yarn via npm: npm install --global yarn
- Create a new Vite project: yarn create vite my-project cd my-project
- Install dependencies: yarn
- Install Dependencies: npm install ethers@5.7.2
- Add Routing: yarn add react-router-dom
- Launch Your Project: yarn run dev

### 2. Deploying Your Contract
- Environment Variables: Enter source .env in your terminal.
- Deploy Script: forge script script/Token.s.sol --rpc-url $RPC_URL --broadcast --private-key $PRIVATE_KEY
- For Sepolia Network: forge script script/Token.s.sol --rpc-url $SEPOLIA_RPC_URL --private-key $SEPOLIA_PRIVATE_KEY --broadcast --verify --etherscan-api-key $ETHERSCAN_API_KEY
- For fuji Network: forge script script/DeployedNFT.s.sol --rpc-url $FUJI_RPC_URL --broadcast --private-key $SEPOLIA_PRIVATE_KEY --verify --etherscan-api-key  $ETHERSCAN_API_KEY  
