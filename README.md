# Vault ethernaut CTF

## Solutions

### R&D explorer
1. Track the transaction hash on Sepolia Etherscan
2. Top right options, click on `Partity`
3. https://sepolia.etherscan.io/vmtrace?txhash=0x23c14de74a0648016441012847f37b8737caa4420c81d6f0257c806ed5a30e50&type=parity
4. Track the `create` specific tx
5. Copy the tx and check it on ethercan
6. Go to `State`
7. https://sepolia.etherscan.io/tx/0x23c14de74a0648016441012847f37b8737caa4420c81d6f0257c806ed5a30e50#statechange
8. Result is in storage 1 -> byte32

### Web3.js
Other quick solution with `web3.js`
1. `await web3.eth.getStorageAt(contract.address, 1)`
