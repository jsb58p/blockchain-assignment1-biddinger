# CS-476-Blockchain-Assignment-1

## How to run the code:

1) While inside the Ubuntu BlockchainVM, open the terminal (Ctrl + Alt + T)

2) Navigate to the folder containing blockchain.js

3) Use the command ` node blockchain.js ` to run the code.

## Sample output:

![console output 1 img](https://github.com/jsb58p/CS-476-Blockchain-Assignment-1/blob/main/console_output1.png?raw=true)

![console output 2 img](https://github.com/jsb58p/CS-476-Blockchain-Assignment-1/blob/main/console_output2.png?raw=true)

![console output 3 img](https://github.com/jsb58p/CS-476-Blockchain-Assignment-1/blob/main/console_output3.png?raw=true)

## Reflection:

What did you learn about hashing and immutability?

Why does Proof-of-Work make blockchains so secure?

What surprised you while coding this?

  A hash is a value created using a one-way function so that it is not reversible. In the context of blockchain, hashes are created based off of the block's contents (the index, timestamp, data, previous hash, and number of attempts to create a valid hash) and are used to create a unique fingerprint for each block. Each block stores the hash of the previous block, creating a chain of blocks. Changing the data of a single block will break the entire chain. This is how blockchain is designed to be immutable. 
  
  The concept of Proof-of-Work revolves around the idea that creating hashes that start with particular values, such as three leading 0s, requires a very specific input data for the creation of hash. The probability of creating a valid hash value is very small depending on the difficulty, so many hashes have to be made through brute-force computational work in order to generate one that is valid. Each generated hash is different due to the changing timestamp and incrementing nonce value used in the input data. Once a valid hash is created, it can be verified by checking that the hash matches the block's content and that the previousHash value matches the hash of the previous block. This creates a system where a potential attacker would have to re-create the entire remainder of the chain if they were able to modify the data of a single block. The only way this is possible is if the attacker is providing the majority of computational power to the blockchain and is able to outpace the Proof-of-Work of all other nodes combined in the network. This is why Proof-of-Work makes blockchains so secure.
  
  I'm amazed by the creativity of the people who were able to invent this technology. I was surprised by the number of attempts it took to create a valid hash and how much the number of attempts varied each time I re-ran the code. Seeing how many hashes were being generated in order to create one that is valid helped me understand how the computational power required to generate so many hashes creates a way of preventing data from being modified by attackers. 
