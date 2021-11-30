# blockchain-developer-bootcamp-final-project

<h3>The project</h3>
Flip Coin is a simple Ethereum dApp where you can bet either on heads or tails and win (or lose) ether.
The result is produced through random number generation and cannot be manipulated.
There are no fees except from miners. 
If a bet is lost, the stake gets stored in the jackpot total, which can be won by any player at random.
The contract is deployed on the Ropsten testnet and therefore all players must use Ropsten to participate.

<h3>Frontend</h3>
http://77.68.119.240/plesk-site-preview/flipcoin.io/https/77.68.119.240/

<h3>Demo / Screen Recording</h3>
https://www.youtube.com/watch?v=jERAmhSGfl4

<h3>Directory Structure</h3>
<ul>
  <li>client: Project's frontend.</li>
<li>contracts: Smart contracts that are deployed in the Ropsten testnet.</li>
<li>migrations: Migration files for deploying contracts in contracts directory.</li>
<li>test: Tests for smart contracts.</li>
  <li>img: Image files and favicons.</li>
  <li>js: Main javascript files for project</li>
  </ul>

<h3>Install</h3>
To run your own Flip Coin instance:

<ol>
  <li>Publish the solidity smart contract using Ethereum Wallet and take note of the contract address. You must deposit funds to the contract, either at publish time or using the contract function depositFunds(). This is required because contract must have funds so users can play.</li>

  <li>Edit CNAME file with the webserver url you intend to use.</li>

  <li>Edit js/main.js and replace the address of the contract.</li>

  <li>Upload DApp files to a webserver. </li>
  <li>Play!</li>
  </ol>

To install the local dependencies run npm install in both the root and frontend directory of the project. To run the frontend, call npm run start in the frontend directory.

To run the contract tests, run ganache-cli (host: 127.0.0.1 port: 8545) and truffle test in the root directory.
  
  <h3>Project contract address</h3>
  https://ropsten.etherscan.io/address/0xe4FbC73f03B5Ae1EAf0Aada6C9Cc596f66BBcCB6
