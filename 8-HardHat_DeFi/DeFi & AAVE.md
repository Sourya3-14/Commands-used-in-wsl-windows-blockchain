###### **DeFi \& AAVE**

to run our tests for getcontract we can use forking instead of using mocks(also you can use a testnet)

forking just copies the chain and runs a local node of that copied data



in blockchain all the data are mostly available on chain so its not hard to get a copy of it



instead of running the whole node and downloading the blockchain which takes a lot of computation power any time we reference any address it uses a api call to the Ethereum node to get the needed contract and run the functions



Pros: Quick,easy,resembles what's on mainnet

Cons: We need an abi. Some contracts are complex to work with



```

networks: {

\&nbsp;   hardhat: {

\&nbsp;     chainId: 31337,

\&nbsp;     // blockConfirmations: 1,

\&nbsp;     forking:{

\&nbsp;       url:MAINNET\\\_RPC\\\_URL

\&nbsp;     }
-------

-------

-------

-------

}

```



yarn hardhat run scripts/aaveBorrow.js



yarn add --dev @aave/core-v3 @aave/periphery-v3 @aave/deploy-v3





**Liquidation -** when you borrowed more money than you put up others can take your collateral in return for them paying your loans



**HealthFactor -** healthfactor beloe 1 you will get liquidated(probably was greater than 1)



even after we repay our debt if we see there will be a tiny amount of debt(~0.0000025usd) still left to repay it we can use uniswap
we can also add the program in our project to programtically convert our etherium into the token (DAI,EURS) and repay the debt

