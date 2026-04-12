# E-voting system based on Blockchain Technology
Decentralised Voting application using Ethereum Network
### Abstract
Building a secure electronic voting system that offers the fairness and privacy of current voting schemes, while providing the transparency and flexibility offered by electronic systems has been a challenge for a long time. In this work-in-progress project, we evaluate an application of blockchain as a service to implement distributed electronic voting systems. The paper proposes a novel electronic voting system based on blockchain that addresses some of the limitations in existing systems and evaluates some of the popular blockchain frameworks for the purpose of constructing a blockchain-based e-voting system. In particular, we evaluate the potential of distributed ledger technologies through the description of a case study; namely, the process of an election, and the implementation of a blockchain-based application, which improves the security and decreases the cost of hosting a nationwide election.
### Dir Structure 

```bash
 
    +---.github
    |          stale.yml
    |
    +---build/contracts
    |                  Election.json
    |                  Migrations.json
    |
    +---contracts
    |            Election.sol
    |            Migrations.sol
    |
    +---migrations
    |             1_initial_migration.js
    |             2_deploy_contracts.js
    |
    +---src
    |      +---css
    |      |      bootstrap.min.css
    |      |      bootstrap.min.css.map
    |      |
    |      +---images
    |      |
    |      +---js
    |      |     app.jss
    |      |     bootstrap.min.jss
    |      |     truffle_contract.jss
    |      |     web3.min.jss
    |      |
    |      +---index.html
    |
    +---test
    |       .gitkeep
    |       election.js
    |
    +---.gitattributes
    |
    +---.gitignore
    |
    +---bs-config.json
    |
    +---LICENCE
    |
    +---package-lock.json
    |
    +---package.json
    |
    +---README.md
    |
    +---truffle-config.json
    

```
## Setup
### Dependencies
<ul>
  <li>NPM: https://nodejs.org</li>
  <li>Truffle: https://github.com/trufflesuite/truffle</li>
  <li>Ganache: http://truffleframework.com/ganache/</li>
  <li>Metamask: https://metamask.io/</li>
</ul>  

Follow the steps below to download, install, and run this project.

Install adn Use brave browser for this project



### Step 1. Clone the project
`git clone https://github.com/rachakonduguruvaishnavi66/E-voting-system-based-on-Blockchain-Technology.git`

### Step 2. Install dependencies
```
$ cd E-voting-system-based-on-Blockchain-Technology
$ nvm use 16
$ npm install
```
### Step 3. Install Truffle
`$ npm install -g truffle`

### Step 4. Start Ganache
Open the Ganache GUI client. This will start your local blockchain instance.


### Step 5. Compile & Deploy Election Smart Contract
`$ truffle migrate --reset`
You must migrate the election smart contract each time your restart ganache.

### Step 6. Configure Metamask

- We are using Metamask version 11.16.1 for this project 
- Download it from here from https://github.com/MetaMask/metamask-extension/releases/tag/v11.16.1
- click on metamask-chrome-11.16.1.zip
- Unzip it
- Go to brave extensions and click on developer mode
- click on load unpack option 
- select the metamask-chrome-11.16.1 folder
- Get started and continue with signing on the metamask old version

- Add a new network with 
Network Name : ganache
New RPC URL : HTTP://127.0.0.1:7545
Chain ID : 1337 
Currency Symbol : ETH

- Unlock Metamask
- Connect metamask to your local Etherum blockchain provided by Ganache.
- Import an account provided by ganache.

- You should see 100 ETH 

### Step 7. Run the Front End Application
`$ npm run dev`
Visit this URL in your browser: http://localhost:3000

- Make sure your metamask acccount is connected to website . After accounts click on globe sign if not connected , click on the 3 dots and go to   - connected sites and enter manually connect

- Refresh it to see the website voter adresss is same as connnected metamask wallet account adress.

-  Refresh to sync website and metamask wallet
 
- Refresh it to get results after voting 

If you get stuck, want to collaborate or found a bug, please raise an issue.
