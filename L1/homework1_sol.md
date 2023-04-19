# Homework 1 / Solution

## Question: Decentralised Systems

> Discuss in your teams what a decentralised version of a game like monopoly would be like, if there was no software on a central server.
> 
> - How would you solve the problems of cheating
> - Ensuring agreement about the state of the system
> - Communication problems (timeouts)
> - How to decide who should take the next turn
> - How to allow the correct people to join the game
>  This is just a general discussion, there is no need to write any code or do any detailed design

## Solution

### How would you solve the problems of cheating

> The rules of the game can be monitored, movement by movement, by establishing a decentralized network, in which case, after each movement, each player reviews the legality of the movement, the state of the other players and the state of the board in general. If an illegal movement is detected, it will not be approved by consensus and must be retracted, preventing its storage in the history of movements


### Ensuring agreement about the state of the system

> Just as a Blockchain network works, there is an agreed consensus mechanism that allows ruling decisions on the network. Likewise, each movement is stored publicly, which allows auditing the legality of each movement through, for example, a block explorer.


### Communication problems (timeouts)

> In general, a blockchain has a much more robust operation than a centralized network architecture, because there are multiple paths in the network through which to establish communication. In any case, since the information is distributed, the players can communicate with each other (which does not present problems) and establish a strategy against the problem through consensus.


### How to decide who should take the next turn

> There are two ways to determine the turn order. On the one hand, if the order is determined by a deterinistic model, this must be specified at the beginning of the game and each player will audit that the public turn allocation process is carried out according to the established rules. On the other hand, if the turn order of each player is determined by a stochastic model, it can be linked to Blockchain Oracles such as Chainlink.


### How to allow the correct people to join the game

A smart contract can be implemented that only allows certain users (wallets) to enter. Another more flexible way is to assign an NFT that gives you the right to enter, and everyone who owns that NFT can enter the game, this NFT can be assigned characteristics such as that it is non-transferable or that a limited number of them can be mited .