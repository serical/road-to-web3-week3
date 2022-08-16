# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a script that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
GAS_REPORT=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
```


### [Contract](https://mumbai.polygonscan.com/address/0x2422e6bb75603b3CC108459F73f2C386eD2F76d2)
```shell script
yarn add @nomiclabs/hardhat-etherscan 

npm install dotenv
npm install @nomiclabs/hardhat-waffle

npx hardhat compile

➜  ChainBattled npx hardhat run scripts/deploy.js --network mumbai
Contract deployed to: 0x2422e6bb75603b3CC108459F73f2C386eD2F76d2


➜  ChainBattled npx hardhat verify --network mumbai 0x2422e6bb75603b3CC108459F73f2C386eD2F76d2
Nothing to compile
Warning: Function state mutability can be restricted to view
  --> contracts/ChainBattles.sol:19:5:
   |
19 |     function generateCharacter(uint256 tokenId) public returns(string memory){
   |     ^ (Relevant source part starts here and spans across multiple lines).


Successfully submitted source code for contract
contracts/ChainBattles.sol:ChainBattles at 0x2422e6bb75603b3CC108459F73f2C386eD2F76d2
for verification on the block explorer. Waiting for verification result...

Successfully verified contract ChainBattles on Etherscan.
https://mumbai.polygonscan.com/address/0x2422e6bb75603b3CC108459F73f2C386eD2F76d2#code
```

