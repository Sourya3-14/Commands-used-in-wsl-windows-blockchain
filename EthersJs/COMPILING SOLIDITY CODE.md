###### **COMPILING SOLIDITY CODE**



**Install corepack-**

sudo npm install -g corepack



**To enable corepack and install yarn pakage manager**

corepack enable
yarn --version



*\*If fails then use*
ls -l $(which corepack)

node /usr/local/lib/node\_modules/corepack/dist/corepack.js enable
yarn  --version



**To install node solc compiler equivalent of yarn-**

yarn add solc

yarn add solc@0.8.7-fixed(use the same version here as used in solidity code)



**Will show all the options solcjs has**
yarn solcjs --help

**Options:**

&nbsp; -V, --version                        output the version number

&nbsp; --version                            Show version and exit.

&nbsp; --optimize                           Enable bytecode optimizer. (default: false)

&nbsp; --bin                                Binary of the contracts in hex.

&nbsp; --abi                                ABI of the contracts.

&nbsp; --standard-json                      Turn on Standard JSON Input / Output mode.

&nbsp; --base-path <path>                   Automatically resolve all imports inside the given path.

&nbsp; -o, --output-dir <output-directory>  Output directory for the contracts.

&nbsp; -h, --help                           output usage information


**To Compile solidity contract-**

yarn solcjs --bin --abi SimpleStorage.sol --include-path node\_modules/ --base-path . -o build/

*\*if fails* 

*node node\_modules/solc/solcjs --bin --abi SimpleStorage.sol --include-path node\_modules/ --base-path . -o build/*



<b>Or you can do-</b>

"scripts":{

&nbsp;   "compile": "yarn solcjs --bin --abi SimpleStorage.sol --include-path node\_modules/ --base-path . -o build/"

&nbsp; }

,add this in pakage.json and running this on terminal will do the same thing now -> yarn compile

