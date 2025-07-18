###### **LINTING**



yarn add --dev solhint



yarn solhint --init



yarn solhint contracts/\*.sol



yarn solhint contracts/\*.sol --fix





###### **COVERAGE**



yarn hardhat coverage





###### **PRETTIER**



yarn add --dev prettier prettier-plugin-solidity



yarn prettier --write .



**create .prettierrc and .prettierignore by yourself**
{

  "tabWidth": 4,

  "useTabs": false,

  "singleQuote": false,

  "semi": false

}



node\_modules/

artifacts/

cache/

out/

dist/

coverage/

\*.abi

\*.bin

\*.lock

.env

\*.json

ignition/deployments

