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



**Programatically verify the contract**
create etherscan acc to get the api key follow hardhat documentation for verify using @nomicfoundation/hardhat-verify
npm install --save-dev @nomicfoundation/hardhat-verify


**And add the following statement to your hardhat.config.js:**

require("@nomicfoundation/hardhat-verify");



**Add this in hardhat.config.js-**

etherscan: {

&nbsp;   // Your API key for Etherscan

&nbsp;   // Obtain one at https://etherscan.io/

&nbsp;   apiKey: "YOUR\_ETHERSCAN\_API\_KEY"

&nbsp; },



**command:** npx hardhat verify --constructor-args arguments.js DEPLOYED\_CONTRACT\_ADDRESS
or you can do this using a separate function in your deploy script(included in hardhat repo)

