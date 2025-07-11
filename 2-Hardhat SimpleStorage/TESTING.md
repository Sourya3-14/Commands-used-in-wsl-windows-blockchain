###### **MORE ON TESTING**



**to run a test for your smart contract (first write a testcode in javascript in test folder then tun using)**

tarn hardhat test



**to run a specific test**

yarn hardhat test --grep <keyword> contained in you it(text,function(){}) text part



***Testing gas price***

add this plugin first - yarn add hardhat-gas-reporter --dev

gasReporter: {

    enabled: true,

},
**add this in config**
***->also you can add other parameters too
then run*** yarn hardhat test ***and will show gas price data on terminal(also can be stored in a file)***

