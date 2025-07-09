###### **HARDHAT**



**initialize using yarn-**
yarn init



**Adding hardhat for development-**

yarn add --dev hardhat



**Initialize hardhat**

npx hardhat init



**if any error occurs probably due to addition of a unwanded .config file somewhere in the project
run this command**
npx hardhat --verbose
**it will locate the file and you can delete it agin initialize**

***run*** npm install ***if any other error showing***



***to use*** yarn hardhat accounts ***add this at the beginning of hardhat.config.js-***

task("accounts", "Prints the list of accounts", async (taskArgs, hre) => {

&nbsp; const accounts = await hre.ethers.getSigners();



&nbsp; for (const account of accounts) {

&nbsp;   console.log(account.address);

&nbsp; }

});

