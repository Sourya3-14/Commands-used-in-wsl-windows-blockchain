###### **DEPLOYING THE SMART CONTRACT**



**Install ganache it will provide us with testnets with 100Eth each same as remix prodied us**



**Install EthersJs**

yarn add ethers



**Add fs-extra**

yarn add fs-extra



**so like the video showed downloading ganache from google and running server will work it will not as you are using linux wsl and running the server on windows to solve this do this**
npm install -g ganache

ganache --port 7545 > ganache.log 2>\&1 \& (adds a file ganache.log which contains the info of nodes)



**then deploy it and it will work (node deploy.js)**

