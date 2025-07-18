###### **FUNDME COMPILING**



**in remix we imported aggregaatorv3interface without any hassale but here we have to download it first**

yarn add --dev @chainlink/contracts ***(will be present in node\_module folder)***

**now use-** yarn hardhat compile





###### **FUNDME DEPLOYING**



**add the hardhat-deploy package for better management-**
yarn add --dev hardhat-deploy



**add this at the top of hardhat.config.js-**

require("hardhat-deploy")



**then create e deploy folder *(previously we used scripts folder to write our deploy.js)***



***then use this to override existing ethers package***

yarn add --dev @nomiclabs/hardhat-ethers@npm:hardhat-deploy-ethers ethers

**now use-** yarn hardhat deploy*(deployes on only hardhat local network)*

	 yarn hardhat deploy --network sepoli*a(can be any name defined in network section of hardhat.config.js properly)*



*to deploy only with specific tags
yarn hardhat deploy --tags <tag\_name>*



###### ***FUNDME VERIFICATION***



*write a veriy scripts in utils folder and import it in yout deploy code and call the function if its testnet or mainnet*

*running yarn hardhat deploy ... will automatically verify then*

