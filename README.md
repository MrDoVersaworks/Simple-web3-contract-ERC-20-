# Simple Web3 Token Contract (ERC-20)

This is a basic implementation of an ERC-20 token smart contract on the Ethereum blockchain. The contract allows users to mint and transfer tokens.

## Technologies Used:
- Solidity
- Ethereum
- Truffle/Hardhat (for deployment)
- MetaMask (for interacting with the contract)

## How to Run:
1. Install [Truffle](https://www.trufflesuite.com/truffle) or [Hardhat](https://hardhat.org/) to compile and deploy the contract.
2. Create a new Ethereum wallet using MetaMask and obtain some test ETH (e.g., from [Ropsten faucet](https://faucet.ropsten.be/)).
3. Compile the contract using `truffle compile` or `npx hardhat compile`.
4. Deploy the contract to a test network using `truffle migrate --network ropsten` or `npx hardhat run scripts/deploy.js --network ropsten`.
5. Interact with the contract through a decentralized app or use Web3.js to call the functions.

## Example Usage:
- Transfer tokens:
```javascript
const token = new web3.eth.Contract(abi, contractAddress);
token.methods.transfer('0xReceiverAddress', amount).send({ from: senderAddress });
