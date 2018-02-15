# Install-truflle-for-Solidity-IDE-
Compiler for Smart Contract Installation step by steps.

## What are Smart Contracts?
Smart contracts are self-executing contracts with the terms of the agreement between buyer and seller being
directly written into lines of code. The code and the agreements contained therein exist across a distributed,
decentralized blockchain network. Smart contracts permit trusted transactions and agreements to be carried
out among disparate, anonymous parties without the need for a central authority, legal system, or external
enforcement mechanism. They render transactions traceable, transparent, and irreversible.


## How Smart Contracts works?
ICO smart contract and tools documentation,This is a documentation for ICO package providing Ethereum smart contracts and command line tools for launching your ICO crowdsale or token offering. ICO stands for a token or cryptocurrency initial offering
crowdsale. It is a common method in blockchain space, decentralized applications for funding of your project.

## Walkthrough:
Features and design goals	
 
## Best practices:  Smart contracts are written with the modern best practices of Ethereum community 
Separation of concerns:  Crowdsale, token and other logic lies in separate contracts that can be  assembled together. 
 Testable:  We aim for 100% branch code coverage by automated test suite  Auditable:  Our tool chain supports verifiable EtherScan.io contract builds 
 Reusable:  The contract code is modularized and reusable across different projects,  all variables are parametrized and there are no hardcoded values or magic numbers 
Refund:  Built-in refund and minimum funding goal protect investors 
Migration:  Token holders can opt in to a new version of the token contract in the case the token owner wants to add more functionality to their token 
Reissuance:  There can be multiple crowdsales for the same token (pre-ICO,  ICO,  etc.) 
Emergency stop:  To try to save the situation in the case we found an issue in the contract post-deploy 
Build upon a foundation:  Instead of building everything from the scratch,  we used Open Zeppelin contracts as much as possible as they are the gold standard of Solidity development. 
Deployment Tool:  We use truffle as the best and the secure framework to deploy or compile the contract.  

# Installation:

Tools for installations (Localhost + Test NET)
•	geth
•	truffle
•	Node JS
•	Node gyp
•	visual studio code (IDE with solidity extension)
•	open Zeppelin library for ICO & Tokens
Localhost, Test Net and Ether Scan
•	https://rinkeby.etherscan.io/address/0x645687FE8e655e8203B3649Ac7f54bc9d657A703
•	Localhost
•	https://etherscan.io/ 
Installation Steps 
•	Install Python 2.7 (https://www.python.org/downloads/)
•	Set Environment Variables for Python i.e. (C:\Python27\)
•	Install Node JS (https://nodejs.org/en/download/)
•	Install Node gyp (with Build Tools)
•	For Node gyp (https://github.com/nodejs/node-gyp)
o	npm install -g node-gyp
o	npm install --global --production windows-build-tools
o	node-gyp --python /path/to/python2.7
o	npm config set python /path/to/executable/python2.7
•	Installing Git (https://git-scm.com/download/) click on windows if you are using Windows
•	Install Truffle 
o	For Installing Truffle (https://github.com/trufflesuite/truffle)
o	https://www.versioneye.com/nodejs/truffle/3.4.11 (Preferable and stable version of truffle)

•	Install chocolatey (https://chocolatey.org/install)
o	Open Windows Power Shell as Administrator and run the following commands
	Set-ExecutionPolicy Bypass -Scope Process
	Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

•	Install Geth on Windows 
o	https://github.com/ethereum/go-ethereum/wiki/Installation-instructions-for-Windows
o	Download zip file
o	Extract geth.exe from zip
o	Open a command prompt
o	Chdir
o	open geth.exe
o	Open Windows Power Shell as an Administrator and run the following commands
o	C:\Windows\system32> choco install git
o	C:\Windows\system32> choco install golang
o	C:\Windows\system32> choco install mingw 
o	Close Power Shell and Reopen Windows Power Shell as a User
o	C:\Users\xxx> set "GOPATH=%USERPROFILE%"
o	C:\Users\xxx> set "Path=%USERPROFILE%\bin;%Path%"
o	C:\Users\xxx> setx GOPATH "%GOPATH%"
o	C:\Users\xxx> setx Path "%Path%"
o	C:\Users\xxx> mkdir src\github.com\ethereum
o	C:\Users\xxx> git clone https://github.com/ethereum/go-ethereum src\github.com\ethereum\go-ethereum
o	C:\Users\xxx> cd src\github.com\ethereum\go-ethereum
o	C:\Users\xxx> go get -u -v golang.org/x/net/context
o	C:\Users\xxx> go install -v ./cmd/...

•	Install Test RPC 
o	https://github.com/ethereumjs/testrpc
	npm install -g ethereumjs-testrpc
	Add Path to system Variable Path
	Close the terminal or restart computer
	Run testrpc command in CMD
•	Install Visual Studio Code
o	Install Solidity Extension
•	Open VSCode
o	Press Ctrl + ~ (CMD will be opened)
o	Run truffle init
o	Run truffle compile
o	Run truffle migrate



What is OpenZeppelin?
OpenZeppelin is a library for writing secure Smart Contracts on Ethereum. OpenZeppelin integrates with Truffle, an Ethereum development environment.

What is Mocha?
Mocha is a feature-rich JavaScript test framework running on Node.js and in the browser, making
asynchronous testing simple and fun. Mocha tests run serially, allowing for flexible and accurate
reporting, while mapping uncaught exceptions to the correct test cases.

What is Chai?
Chai is a BDD / TDD assertion library for node and the browser that can be delightfully paired with
any JavaScript testing framework.

How to run an ICO smart contracts?
1.	Create a new folder
2.	Open it with VS Code
3.	Open terminal (Ctrl + `)
4. Run following commands:
4.1.	npm init
4.2.	truffle init
4.3.	npm install zeppelin-solidity –save
4.4.	npm install truffle-hdwallet-provider –save
5.	To compile code: truffle compile 
6.	To test code: truffle test
7.	To migrate code: truffle migrate 
7.1.	Networks:
7.1.1.	Development (testrpc) 
7.1.2.	Rinkeby (Test network)
7.1.3.	Main (Main network)
7.2.	–reset (Used to recompile all code)
7.3.	Complete command: truffle migrate –network development –reset



Project Cleanup Tips:
•	Delete the sample files except Migrations.sol
•	Delete the contents of 2_deploy_contracts.js
 


Test Driven Development:

Network
