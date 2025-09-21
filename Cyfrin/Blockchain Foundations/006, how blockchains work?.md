
## core ideas
- block, nonce , data => produce a unique hash 
- the miners of different blockchain usually solve a problem where they have to find a particular value of nonce for which the produced hash fulfills a certain condition. these three values are used to produce a hash. 
- as a result, even a minor change in the data leads to an entirely different hash, hence, invalidating the block.
- **Genesis block** : this is the first block in the blockchain. 
- If there was a single entity that was controlling blockchain, it would not be much different than a single server storing data; so the catch comes in as distributed system. 

## public and private keys 
- a private key is a randomly generated key used to sign all transactions. 
- private key is then passed through ECDSA hashing algorithm to create the corresponding public key. 
- **the private must remain secret and the public key is accessible for verification by design**; revealing private key can be insanely costly (actually depending on the amount of funds)
- private key + message = message signature ; it is impossible to derive the private key from the message signature (at least for now)
- anyone can verify the message signature using the user's public key. 
- interesting side note: the wallet addresses are derived from public keys.


## gas in depth
- base fee : the min *gas price* to send your transactions. 
- whenever we send a transaction on ethereum,  a part of it is completely removed , it is termed as **burnt**. 
- the most important thing is that sending transactions get more expensive as more people use the chain. 

## blockchain overview
### consensus
- this is very important idea in context of blockchains; this is the mechanism by which nodes or participants agree on the state of the blockchain. 
- PoW and PoS are two of the most common consensus algorithms. 
- very important ideas for a consensus
	- chain selection 
	- sybil resistance 
- Proof of Work is known as a **Sybil Resistance Mechanism**
- Sybil Resistance is a blockchain's ability that allows it to defend itself from users creating large number of fake nodes (I know this is highly inaccurate, but I am trying to phrase it whatever I am understanding)
- To simplify Sybil Resistance, it is blockchain's measure so that users don't create fake nodes to receive rewards (still a lot of questions)

## Proof of Work
- PoW is Sybil resistant because each node has to go through a a very computationally intensive process called mining. 
- block confirmations: these are simply new blocks added after our transaction has been merged in the blockchain. 



