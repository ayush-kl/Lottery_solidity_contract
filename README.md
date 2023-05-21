# Solidity Lottery Contract

This project implements a lottery contract using Solidity. Participants can join the lottery by paying 1 ether each, and the winner of the lottery will receive the entire prize pool. The contract is managed by a designated manager.

## Contract Details

The lottery contract consists of the following components:

- **Lottery Contract:** Manages the overall functionality of the lottery.
- **Participants:** Individuals who pay 1 ether to join the lottery.
- **Manager:** The designated manager who oversees the lottery process and selects the winner.
- **Winner:** The participant who wins the lottery and receives the entire prize pool.

## Contract Functions

The following functions are available in the lottery contract:



### `getBalance()`

Returns the current total amount of ether collected in the prize pool.


### `random()`

Generating a long random number that is used to get a random index of participant that wins the lottery.


### `selectWinner()`

Only the manager can execute this function. It randomly selects a winner from the list of participants and transfers the entire prize pool to the winner.





## Getting Started

To deploy and interact with the lottery contract, follow these steps:

1. Install a Solidity development environment such as Remix or Truffle.
2. Compile the `lottery.sol` file.
3. Deploy the contract to the Ethereum network of your choice.
4. Set the manager address in the deployed contract to specify the manager of the lottery.
5. Through Recieve participants can send 1 ether and get joined.
6. Once enough participants have joined, the manager can call the `selectWinner()` function to choose the winner.
8. 

## Notes

- Ensure that the manager address is set correctly before starting the lottery.
- Be cautious when interacting with the contract to prevent any unauthorized access or loss of funds.
- Ensure that the no. of participants is greater or equal to 3.

## Disclaimer

This project is provided as-is without any warranties or guarantees. Use it at your own risk. The authors and contributors are not responsible for any losses or damages incurred.