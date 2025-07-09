###### [***WSL SETUP FOR WINDOWS TO USE LINUS ENVIROMENT***](https://learn.microsoft.com/en-us/windows/wsl/install)



**Installing WSL in windows-**

wsl --install



**If failed then run these commands-**

dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart

dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

dism.exe /online /enable-feature /featurename:HypervisorPlatform /all /norestart

dism.exe /online /enable-feature /featurename:Hyper-V /all /norestart



*\*Last command may show some error ignore it and run this again*

wsl --install -d Ubuntu





**Now on VsCode-**

* install Remote Devnet extension
* ctrl + shift + p
* remote explorer: focus on wsl target view or in side bellow extensions remote explorer will be available choose from there



*\*If on VsCode terminal ubuntu is not open then not correct ask chatgpt*



**To install Node.js in ubuntu-**

* create a folder and move to it
* curl  -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
* trach the terminal then reopen it
* nvm --version (if shows version then correctly installed)



**Check if git installed-**
git --version



**To install NodeJs-**

sudo apt install nodejs npm



**To run javascript code-**
node <filename>.js

