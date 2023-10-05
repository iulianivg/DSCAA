# DSCAA - Deploy smart contracts as an agency

Do you own a web3 agency and deploy many smart contracts? Some of your clients have certainly been accused of running a scam or whatever. 
They will point to your address as "the bad address" when you have nothing to do with the business, but being a developer. 

This standard allows you to deploy smart contracts, and declare that you are a web3 agency on chain. At the moment of deployment you will pass your company's website which
will be emmited as an event.

The smart contract is already deployed on these chains: 

- Ethereum [0x4370ada30598EF7494f8F3DAC9dc82843b25Fa95](https://etherscan.io/address/0x4370ada30598ef7494f8f3dac9dc82843b25fa95#code)
- BSC [0x6ce418e39feb5272b5ab42a1e5d2765521107474](https://bscscan.com/address/0x6ce418e39feb5272b5ab42a1e5d2765521107474#code)
- Polygon [0x526956E802007C6512FbfeE192CC7ACbC4EaD174](https://polygonscan.com/address/0x526956E802007C6512FbfeE192CC7ACbC4EaD174#code)


## Instructions for running
Your smart contract must take NO parameters as a constructor. We recommend Initialize pattern instead, so that you can call "initialize" via `invokeMethod`. 

Here is an example using [remix.ethereum.org](https://remix.ethereum.org/)

1. Get the Token.sol contract from this repository and paste it in Remix
2. Compile using solidity 0.6.12
3.  ![image](https://github.com/iulianivg/DSCAA/assets/43420841/6332cdc3-8bf8-4b67-aeec-c7dee7218c42)
4.  Select "Token" which is the smart contract being deployed
5.  ![image](https://github.com/iulianivg/DSCAA/assets/43420841/bea25d15-cdf1-428d-9d65-73a20c5b24c2)
6.  Copy the ByteCode
7.  ![image](https://github.com/iulianivg/DSCAA/assets/43420841/3efe7d3c-f76c-45f5-806b-418de298bf46)
8.  Visit the DSCAA smart contract on the chain you want to deploy.
9.  Add "0x" at the beggining of the copied bytecode and paste it. Also type in your web3 agency website.
10.  ![image](https://github.com/iulianivg/DSCAA/assets/43420841/1c7e6010-53ca-42e6-b286-b008b7a597b2)
11.  Congratulations! You have deployed your token. Inspect the transaction to get the address of the deployed smart contract. 
12.  ![image](https://github.com/iulianivg/DSCAA/assets/43420841/2f39dc2a-8b11-47fd-9b42-b079332cd2e5)
13.  Want to call a method on your smart contract? Simply use invokeMethod. Ideally you'll want to transfer ownership to yourself if your smart contract has "owner". 
14.  ![image](https://github.com/iulianivg/DSCAA/assets/43420841/9bb23e72-aa9a-43f4-8dd7-acfe6edb7589)



## Improvements
One way to improve DSCAA is by allowing constructor parameters to be passed at deployment time. To be done.

