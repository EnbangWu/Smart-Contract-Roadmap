# Smart-Contract-Auditor-Roadmap
This is a personal smart contract auditor roadmap, including textbooks, articles, videos and best practice examples. The goal of this roadmap is to help me understand smart contrac , cryptography, security best practices and gas optimization. I hope this roadmap can also help you.
TODO:<br>
- [ ] Develop state of the art smart contract security analysis tools.<br> better be fuzzer 
- [ ] Find high risk bug on Code4rena
- [ ] learn Yul


## Helpful combo 
[Blockchain security & audit by consensys](https://consensys.net/diligence/)
## Books
- [x] [mastering Ethereum](https://github.com/ethereumbook/ethereumbook)
<br>This book is a must read and it helps me clarify most fundemental concepts related to blockchain, Ehtereum, EVM. It also touches the creation of solidity and vyper. 5:star:/5:star:. <br>
[notes on mastering Ethereum](https://adhesive-cowl-245.notion.site/Mastering-Ethereum-Building-Smart-Contracts-and-Dapps-373249b998a94b71bb6c8dd87a255a6c)

- [x] [Introduction to Modern Cryptography](http://staff.ustc.edu.cn/~mfy/moderncrypto/reading%20materials/Introduction_to_Modern_Cryptography.pdf) <br> This is the textbook of my Direcy reading program in our math department. It walks me through from symmetric encryption to asymmetric encryption. I have learned about Sha3(keccak), merkle trees, Verfiable secret sharing,etc. <br> TODO: notes
## Blogs
- [x] [Reentrancy Attack](https://gus-tavo-guim.medium.com/reentrancy-attack-on-smart-contracts-how-to-identify-the-exploitable-and-an-example-of-an-attack-4470a2d8dfe4)
- [x] [Smart contract security audit](https://www.blockchain-council.org/blog/smart-contract-security-audit) <br> Introduced the process of smart contract security audit lifecycle, and the common vulnerabilities. <br>
- [x] [Analysis of the Dao exploit](https://hackingdistributed.com/2016/06/18/analysis-of-the-dao-exploit/)
- [x] [Write Rust lints without forking Clippy](https://www.trailofbits.com/post/write-rust-lints-without-forking-clippy) <br> This is a tutorial of how to write a custom lint for Rust. How Dylint groups linters together an dprevent the drawbacks of Clippy. Ready to jump right in Dylint! <br>
- [x] [How to do smart contract security audit](https://blaize.tech/article-type/how-to-conduct-a-smart-contract-security-audit-of-your-project-and-why-this-is-important/)

## Codebase reviewd


## EVM
Contributed to this open source EVM project: [yet another EVM puzzle](https://github.com/mattaereal/yet-another-evm-puzzle/tree/main/puzzles)
- [x] [Deconstruct a solidity contract](https://blog.openzeppelin.com/deconstructing-a-solidity-contract-part-i-introduction-832efd2d7737/)<br>Introduction of how a solidity smart contract is converted into opcodes
- [x] [Creation VS runtime](https://blog.openzeppelin.com/deconstructing-a-solidity-contract-part-ii-creation-vs-runtime-6b9d60ecb44c/)<br> Talks about creation-time code and runtime code, creation time code will load function parameters, copy runtime code to memory, and then jump to runtime code.
## Ethernut Challenges 
My solutions of Ethernaut Challenges: [solutions](https://github.com/EnbangWu/CTF-solutions/tree/main/Ethernaut)
- [x] [Fallback](https://ethernaut.openzeppelin.com/level/0x9CB391dbcD447E645D6Cb55dE6ca23164130D008) <br> A nice and smooth intro to the Ethernaut challenges. Including useage of ethers,fallback functions and ownership. Takeaway: Never change ownership or something private in the fallback functions!
- [x] [Fallout](https://ethernaut.openzeppelin.com/level/0x5732B2F88cbd19B6f01E3a96e9f0D90B917281E5) <br>A simple spelling error that could destroy the whole smartt contract! 
- [x] [CoinFlip](https://ethernaut.openzeppelin.com/level/0x4dF32584890A0026e56f7535d0f2C6486753624f)<br> A vulnerble smart contract that uses the self-defined random number generator. Should use the oracle to generate the randomness.
- [x] [Telephone](https://ethernaut.openzeppelin.com/level/0x1ca9f1c518ec5681C2B7F97c7385C0164c3A22Fe)<br> Tx.origin != msg.sender
- [x] [Token](https://ethernaut.openzeppelin.com/level/0x1ca9f1c518ec5681C2B7F97c7385C0164c3A22Fe)<br> arithmatic underflow
- [x] [Delegation](https://ethernaut.openzeppelin.com/level/0x1ca9f1c518ec5681C2B7F97c7385C0164c3A22Fe)<br> Delegate call
- [x] [Force](https://ethernaut.openzeppelin.com/level/0x1ca9f1c518ec5681C2B7F97c7385C0164c3A22Fe)<br> Force sending thorugh selfdestruct
- [x] [Valut](https://ethernaut.openzeppelin.com/level/0x3A78EE8462BD2e31133de2B8f1f9CBD973D6eDd6)<br> Private variable is readble
- [x] [King](https://ethernaut.openzeppelin.com/level/0x725595BA16E76ED1F6cC1e1b65A88365cC494824)<br> Always checking the invariant of the smart contract
- [x] [Re-entrancy](https://ethernaut.openzeppelin.com/level/0x1ca9f1c518ec5681C2B7F97c7385C0164c3A22Fe)<br> Re-entrancy, use the pull payments if possible
- [x] [Elevator](https://ethernaut.openzeppelin.com/level/0x4A151908Da311601D967a6fB9f8cFa5A3E88a251)<br> Don't trust unknowen contracts
- [x] [Privacy](https://ethernaut.openzeppelin.com/level/0xcAac6e4994c2e21C5370528221c226D1076CfDAB)<br> Private variable is readble
- [x] [GatekeeperOne](https://ethernaut.openzeppelin.com/level/0x2a2497aE349bCA901Fea458370Bd7dDa594D1D69)<br> gasleft() and typecasting
- [x] [GatekeeperTwo](https://ethernaut.openzeppelin.com/level/0xf59112032D54862E199626F55cFad4F8a3b0Fce9)<br> creation time code and runtime code, bitwise operation
- [x] [NaughtCoin](https://ethernaut.openzeppelin.com/level/0x36E92B2751F260D6a4749d7CA58247E7f8198284)<br>Inheritate the contract incorrecly
- [x] [Preservation](https://ethernaut.openzeppelin.com/level/0x2754fA769d47ACdF1f6cDAa4B0A8Ca4eEba651eC)<br> Delegate call and storage layout
  

## Published Articles
[Medium articles ](https://medium.com/@0xNorman)