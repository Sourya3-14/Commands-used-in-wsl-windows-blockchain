###### **FUNDME TESTING**



**to test your deployed contract**

yarn hardhat test

**to run a specific test**

yarn hardhat test "test/staging/FundMe.staging.test.js" --network sepolia 

**to run test based on a specific network**          

yarn hardhat test --network sepolia    





###### **RUNNING ON A LOCAL NODE**

yarn hardhat node it will automatically deploy your code in a a local network and also provide the RPC url and address where the contract is deployed and also list of accounts associated with that node





###### **ADDING SCIPTS ON YOUR pakage.json**

 "scripts": {

&nbsp;   "test": "yarn hardhat test",

&nbsp;   "test stage": "yarn hardhat test --network sepolia",

&nbsp;   "lint": "yarn solhint contracts/\*.sol",

&nbsp;   "lint:fix": "yarn solhint contracts/\*.sol --fix",

&nbsp;   "format": "yarn prettier --write .",

&nbsp;   "coverage": "yarn hardhat coverage"

&nbsp; }

**running** yarn <...> **will do the same now**



