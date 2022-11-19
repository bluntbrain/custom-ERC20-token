# custom-ERC20-token

https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol</br></br>

ERC stands for Ethereum Request for Comment. Essentially, they are standards that have been approved by the community and are used to convey technical requirements and specifications for certain use cases.</br></br>


import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol"; </br>

This line imports the ERC-20 token standard from OpenZeppelin (OZ). OZ is an Ethereum security company. Among other things, OZ develops reference contracts for popular smart contract standards which are thoroughly tested and secure. Whenever implementing a smart contract which needs to comply with a standard, try to find an OZ reference implementation rather than rewriting the entire standard from scratch.</br></br>

Essentially, Solidity does not support floating point numbers - that is decimals. Also, since ERC20 tokens deal with money, using floating point numbers is a bad idea.</br>

ERC20 tokens by default work with 18 decimal places. So 1 full LW3Token in this case, is actually represented as 10 ^ 18. Therefore, to get 10 full LW3Tokens, we use 10 * 10 ** 18.</br>

```shell
0xC4F5a1659C2DCCb7da1213f7b3CaFcD43A07ca56
```

https://goerli.etherscan.io/tx/0xcda0b9c1f1ee0f3c3c2162fcfe249bd9f7012a48f177dc069aedf6347c272dbf</br>

Hardhat commands</br>
```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat run scripts/deploy.js
```

Command to deploy </br>
```shell
npx hardhat run scripts/deploy.js --network goerli
```

NFT Contract Address: </br>
```shell
0x2AbbbfF1169E825Ab51F80BeFb2899d291505f61
```