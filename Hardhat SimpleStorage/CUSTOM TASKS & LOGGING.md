###### **CREATING CUSTOM TASKS AND SEE LOGGING**



**to run a custom task defined by you-**
yarn hardhat <task\_name>





**to run a local hardhat node in your pc-**
yarn hardhat node




**to see logging output also change hardhat.config.js like this-**
module.exports = {

&nbsp; defaultNetwork: "hardhat",

&nbsp; solidity: "0.8.8",

&nbsp; networks: {

&nbsp;   sepolia: {

&nbsp;     url: SEPOLIA\_RPC\_URL,

&nbsp;     accounts: \[PRIVATE\_KEY],

&nbsp;     chainId: 11155111,

&nbsp;   },

&nbsp;   localhost: {

&nbsp;     url: "http://127.0.0.1:8545/",

&nbsp;     chainId: 31337,

&nbsp;   }

&nbsp; },

&nbsp; etherscan: {

&nbsp;   apiKey: ETHERSCAN\_API\_KEY,

&nbsp; },

};



**run like this-**

yarn hardhat run scripts/deploy.js --network localhost 

