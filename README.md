<h1>Getting a .test name on Ropsten<h1>

1. Download MetaMask
2. Copy the contents of ensutils-testnet-ethdenver and paste it into the web console
3. Check if your name is taken
```
testRegistrar.register(web3.sha3('nameYouWant'), '<MetaMask address>', (err,res)=>console.log(err,res))
```
4. Register your name
```
testRegistrar.register(web3.sha3('nameYouWant'), '<MetaMask address>'))
```
5. Check if your name has been registered on Etherscan.

To resolve to IPFS records:

6. Set the resolver to the public resolver
```
ens.setResolver(namehash('nameYouWant.test'), publicResolver.address, (err,res)=>console.log(err,res))
```
7. Go to tetratorus.github.io to set the IPFS hash to point to

8. Download the ENS Content Resolver (.test) Chrome Extension


Shout out to Philip Prophet (github.com/monkybrain) for letting me use his source code
for the ENS-IPFS resolution tools.
https://github.com/monkybrain/ipfs-to-ens
https://github.com/monkybrain/ens-content-resolver
