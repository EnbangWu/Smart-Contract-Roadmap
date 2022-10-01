# Smart-Contract-Roadmap
This is a personal smart contract developer roadmap, including textbooks, articles, videos and best practice examples.

## Books
- [x] [mastering Ethereum](https://github.com/ethereumbook/ethereumbook)
<br>This book is a must read and it helps me clarify most fundemental concepts related to blockchain, Ehtereum, EVM. It also touches the creation of solidity and vyper. 5:star:/5:star:. <br>
[notes on mastering Ethereum](https://adhesive-cowl-245.notion.site/Mastering-Ethereum-Building-Smart-Contracts-and-Dapps-373249b998a94b71bb6c8dd87a255a6c)

- [ ] [Introduction to Modern Cryptography](http://staff.ustc.edu.cn/~mfy/moderncrypto/reading%20materials/Introduction_to_Modern_Cryptography.pdf) <br> This is the textbook of my Direcy reading program in our math department. It walks me through from symmetric encryption to asymmetric encryption. I have learned about Sha3(keccak), merkle trees, Verfiable secret sharing,etc. <br> TODO: notes

## Blogs
- [x] [Reentrancy Attack](https://gus-tavo-guim.medium.com/reentrancy-attack-on-smart-contracts-how-to-identify-the-exploitable-and-an-example-of-an-attack-4470a2d8dfe4)
- [ ] [Analysis of the Dao exploit](https://hackingdistributed.com/2016/06/18/analysis-of-the-dao-exploit/)
- [ ] [PoWHC and Batch Transfer Overflow](https://medium.com/@ebanisadr/how-800k-evaporated-from-the-powh-coin-ponzi-scheme-overnight-1b025c33b530)

## Ethernut Challenges
- [x] [Fallback](https://ethernaut.openzeppelin.com/level/0x9CB391dbcD447E645D6Cb55dE6ca23164130D008) <br> A nice and smooth intro to the Ethernaut challenges. Including useage of ethers,fallback functions and ownership. Takeaway: Never change ownership or something private in the fallback functions!
- [x] [Fallout](https://ethernaut.openzeppelin.com/level/0x5732B2F88cbd19B6f01E3a96e9f0D90B917281E5) <br>A simple spelling error that could destroy the whole smartt contract! 
- [ ] [CoinFlip](https://ethernaut.openzeppelin.com/level/0x4dF32584890A0026e56f7535d0f2C6486753624f)<br> A vulnerble smart contract that uses the self-defined random number generator. Should use the oracle to generate the randomness.
  
## Dapps Development