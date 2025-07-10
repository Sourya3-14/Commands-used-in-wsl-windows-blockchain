###### **DEPLOYING A SMARCONTRACT IN HARDHAT**



yarn hardhat run scripts/filename.js



***running the script on a specific network-***

yarn hardhat run scripts/deploy.js --network hardhat

**or,**

yarn hardhat run scripts/deploy.js --network sepolia



**add this in hardhat.config.js**
module.exports = {

  defaultNetwork: "hardhat",

  networks: {

    sepolia: {

      url: SEPOLIA\_RPC\_URL,

      accounts: \[PRIVATE\_KEY],

      chainId: 11155111,

    },

  },

  solidity: "0.8.8",

};



**to add dotenv**

yarn add --dev dotenv

