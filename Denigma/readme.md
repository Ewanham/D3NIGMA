### Installation:

**a) Deploy a new contract:**
- Using Foundry :
	1) forge init new_project
  	2) forge install openzeppelin/openzeppelin-contracts --no-commit
  	3) forge install smartcontractkit/chainlink-brownie-contracts@0.6.1 --no-commit
  	4) Import dNFT.sol and DeployedNFT.s.sol
  	5) Update .env
  	6) forge script script/DeployedNFT.s.sol --rpc-url $FUJI_RPC_URL --private-key $SEPOLIA_PRIVATE_KEY --broadcast --verify --etherscan-api-key $ETHERSCAN_API_KEY
  	7) Create a subscription : https://vrf.chain.link/sepolia/ and add a consumer address (Contract address)
  	8) Create a new Upkeep : https://automation.chain.link/sepolia/ and use Custom logic
  	9) Create a new Upkeep with Time-based to call updateBetScore(0)
  	10) Setup CCIP :
  	      1) Deploy Receiver Contract (dNFT) 
  	      2) Deploy Sender Contract and write on it the receiver address.
  	      3) Fund with link the Sender Contract
  	      4) You can stack your token. Just verify.

**b) Run the site:**
- Denigma-site: To run the site, please visit the following folder, detailed instructions, and more.