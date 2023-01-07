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
- [ ] [Deconstruct a solidity contract](https://blog.openzeppelin.com/deconstructing-a-solidity-contract-part-i-introduction-832efd2d7737/)<br>
- [ ] [How to do smart contract security audit](https://blaize.tech/article-type/how-to-conduct-a-smart-contract-security-audit-of-your-project-and-why-this-is-important/)

## Codebase reviewd


## EVM
Contributed to this open source EVM project: [yet another EVM puzzle](https://github.com/mattaereal/yet-another-evm-puzzle/tree/main/puzzles)
## Ethernut Challenges 
My solutions of Ethernaut Challenges: [solutions](https://github.com/EnbangWu/CTF-solutions/tree/main/Ethernaut)
- [x] [Fallback](https://ethernaut.openzeppelin.com/level/0x9CB391dbcD447E645D6Cb55dE6ca23164130D008) <br> A nice and smooth intro to the Ethernaut challenges. Including useage of ethers,fallback functions and ownership. Takeaway: Never change ownership or something private in the fallback functions!
- [x] [Fallout](https://ethernaut.openzeppelin.com/level/0x5732B2F88cbd19B6f01E3a96e9f0D90B917281E5) <br>A simple spelling error that could destroy the whole smartt contract! 
- [x] [CoinFlip](https://ethernaut.openzeppelin.com/level/0x4dF32584890A0026e56f7535d0f2C6486753624f)<br> A vulnerble smart contract that uses the self-defined random number generator. Should use the oracle to generate the randomness.
- [x] [Telephone](https://ethernaut.openzeppelin.com/level/0x1ca9f1c518ec5681C2B7F97c7385C0164c3A22Fe)<br> Tx.origin != msg.sender
- [x] [Token](https://ethernaut.openzeppelin.com/level/0x1ca9f1c518ec5681C2B7F97c7385C0164c3A22Fe)<br> arithmatic underflow
- [x] [Delegation](https://ethernaut.openzeppelin.com/level/0x1ca9f1c518ec5681C2B7F97c7385C0164c3A22Fe)<br> Delegate call
- [x] [Force](https://ethernaut.openzeppelin.com/level/0x1ca9f1c518ec5681C2B7F97c7385C0164c3A22Fe)<br> Force sending thorugh selfdestruct
  

## Published Articles
[Medium articles ](https://medium.com/@0xNorman)