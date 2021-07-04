# About SAS

The full name of SAS is Super Smart Application System. It uses Byzantine Fault Tolerance - Deligated Proof of Stake consensus mechanism to build a decentralized application system

SAS is base on [go-ethereum (v1.7.4)](https://github.com/ethereum/go-ethereum), the onsensus algorithm it is a simple version of DPOS-PBFT consensus algorithm.

We also use header.extra to record the all infomation of current block and keep signature of miner. The snapshot keep vote & confirm information of whole chain, which will be update by each Seal or VerifySeal. By the end of each loop, the miner will calculate the next loop miners from the snapshot.

Developers can configure SAS Mainnet on the development tools to create smart contracts.

#### SAS Mainnet
* [mainnet](https://www.sasmainnet.com): `SAS Mainnet URL`
* [networkid](): `40987`
* [browser](http://www.sasscan.com): `SAS blockchain browser`

The total SAS issuance is 96 million, of which 30% is used for the maintenance of the super nodes and 70% is used for applications.
The super nodes will be rewarded with 2 SAS per block after the launch. After the public network goes online, the candidates for the super node election must hold a total issue of
Candidates for the super node election must hold five ten thousandths of the total issue, which is 48000 SAS.

Translated with www.DeepL.com/Translator (free version)

#### To Support Ethereum Development Tool

SAS support Ethereum development tools, like web3.js, but SAS address it's not prefixed with `0x` like Ethereum, so developer will add prefix `0x` if you use like web3.js

if you have address on SAS it's `0000000000000000000000000000000000000001`, and you want to send a transaction to `0000000000000000000000000000000000000002`, then you can do it like below

```javascript
let rawTransaction = {
    "from": "0x0000000000000000000000000000000000000001",
    "nonce": 1,
    "gasPrice": 40,
    "gasLimit": 121000,
    "to": '0x0000000000000000000000000000000000000002',
    "value": 10,
    "data": ''
}; 
```

#### Other Documents List

* [go-ethereum](https://github.com/ethereum/go-ethereum): `The go-ethereum project `
* [solidity](https://github.com/ethereum/solidity)  : `Solidity, the Contract-Oriented Programming Language`
* [remix](https://github.com/ethereum/remix-ide): `Browser-Only Solidity IDE and Runtime Environment`
* [web.js](https://github.com/ethereum/web3.js): `Ethereum JavaScript API`
* [web3.py](https://github.com/ethereum/web3.py): `A python interface for interacting with the Ethereum blockchain and ecosystem`
* [web3j](https://github.com/ethereum/web3.py): `Lightweight Java and Android library for integration with Ethereum clients`
* [web3.php](https://github.com/sc0Vu/web3.php): `A php interface for interacting with the Ethereum blockchain and ecosystem.`
* [metamask](https://metamask.io/): `MetaMask is an extension for accessing Ethereum enabled distributed applications, or "Dapps" in your normal Chrome browser!`

SRT Protocol
SRT is an intelligent contract protocol developed based on the SAS system.
SAS is named a new generation of BFT-DPOS decentralized application
platform, which supports Turing’s complete intelligent contract and SRT
protocol. At the same time, it supports all the intelligent contracts of Ethereum,
and it also supports the implementation of DAPP with high-performance
consensus to build blockchain 5.0 era.
SRT protocol standard
As a new generation of token embodiment of Token Economy, SRT has
the following standards:
Method
1. name
function name() constant returns (string name)
The name of Token with the type of returning string, such as SAS
2. symbol
function symbol() constant returns (string symbol)
The symbol of Token with the type of returning string is the abbreviation
SAS Whitepaper
24 / 53
of Token, such as SAS.
3. decimals
function decimals() constant returns (uint8 decimals)
It supports a few decimal places behind the decimal point. If it is set as 3,
it will support 0.001.
4. total Supply
function totalSupply() constant returns (uint256 total Supply)
The total number of Tokens issued can be obtained through this function.
The total number of all Token certificates issued by the smart contract is
fixed, so the the initial value must be set for totalSupply.
5. balanceOf
function balanceOf(address _owner) constant returns (uint256 balance)
Enter the address to get the number of Tokens.
6. transfer
function transfer(address _to, uint256 _value) returns (bool success)
Call the transfer function to transfer your own token to the _to address,
and _value is the number of transfers.
7. approve
function approve(address _spender, uint256 _value) returns (bool
success)
Approve the _spender account to transfer _value tokens from your own
account. It can be transferred for multiple times.
8. transferFrom
function transferFrom(address _from, address _to, uint256 _value)
returns (bool success)
It is used in conjunction with approve, while call the transferFrom
function to transfer the token after approved.
9. allowance
function allowance(address _owner, address _spender) constant returns
(uint256 remaining)
Returning _spender can also extract the number of tokens.
