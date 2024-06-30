# Token Smart Contract

This repository contains a simple smart contract for a token system written in Solidity.

## Overview

The `Token` smart contract allows users to manage their token holdings. Users can increase or decrease their holdings and check their current balance.

## Features

- **Increase Holdings**: Users can increase their token holdings by calling the `increaseHoldings` function.
- **Decrease Holdings**: Users can decrease their token holdings by calling the `decreaseHoldings` function, provided they have sufficient balance.
- **View Holdings**: Users can check their current token balance by calling the `viewHoldings` function.

## Contract Details

### Functions

- `increaseHoldings(uint256 amount)`: Increases the token holdings of the caller by the specified amount and emits a `Movement` event.
- `decreaseHoldings(uint256 amount)`: Decreases the token holdings of the caller by the specified amount, provided the caller has enough tokens, and emits a `Movement` event.
- `viewHoldings(address owner)`: Returns the current token balance of the specified address.

### Events

- `Movement(address indexed sender, address indexed receiver, uint256 amount)`: Emitted when tokens are increased or decreased.

## Usage

To interact with the smart contract, you can use any Ethereum development environment like Remix, Hardhat, or Truffle. Below is an example of how you might deploy and interact with the contract using Remix.

### Deploying the Contract

1. Open [Remix](https://remix.ethereum.org/).
2. Create a new file and copy the `Token` contract code into it.
3. Compile the contract using the Solidity compiler.
4. Deploy the contract to the Ethereum network of your choice (e.g., a local development network or a testnet).

### Interacting with the Contract

Once deployed, you can interact with the contract functions through the Remix interface:

- Call `increaseHoldings` with an amount to increase your token balance.
- Call `decreaseHoldings` with an amount to decrease your token balance.
- Call `viewHoldings` with an address to check the token balance of that address.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## Contact

For any questions or inquiries, please contact [Shaanreiforyou@gmail.com].

