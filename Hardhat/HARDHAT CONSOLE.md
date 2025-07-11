###### **HARDHAT CONSOLE**



**to create a console**
yarn hardhat console --network localhost

*(make sure the localhost node is running in your pc mentioned in logging file how to do)*

*also works for "--network hardhat,sepolia" any thing*



**this will open up a shell where you can run any like of your code separately like**



> const SimpleStorageFactory = await ethers.getContractFactory("SimpleStorage")

undefined

>  const simpleStorage = await SimpleStorageFactory.deploy()

undefined

> await simpleStorage.retrieve()

0n

> await simpleStorage.store(255)

(some big output)

> await simpleStorage.retrieve()

255n



