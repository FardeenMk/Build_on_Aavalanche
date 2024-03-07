# PrizeToken

## Overview
The PrizeToken contract is an ERC20 token that allows users to redeem their tokens for different prize levels - Gold, Silver, and Bronze. Users can mint new tokens, burn tokens to redeem prizes, transfer tokens, and get the cost of each prize. The contract is implemented in Solidity and follows the ERC20 standard.

## Functionality
- **Minting Tokens**: Only the contract owner can mint new tokens. Tokens are minted and sent to the specified address.
- **Burning Tokens**: Users can burn their tokens to redeem prizes. The number of tokens burned corresponds to the cost of the chosen prize.
- **Redeeming Prizes**: Users can redeem prizes by burning tokens. The cost of each prize is predefined and deducted from the user's token balance.
- **Transferring Tokens**: Users can transfer tokens to other addresses.

## Contract Structure
The contract is structured as follows:
- `PrizeToken`: The main contract that inherits from `ERC20` and `Ownable`. It defines the token functionalities.
- `Prize`: An enum defining the different prize levels - GOLD, SILVER, and BRONZE.
- `user_Selected_Prizes`: A mapping to keep track of the prize selected by each user.
- `prize_Costs`: A mapping to store the cost of each prize.
- `constructor`: Initializes the contract with the initial owner and sets the initial prize costs.
- `mint`: Function to mint new tokens.
- `burn`: Function to burn tokens for prize redemption.
- `redeem_Prize`: Function to redeem prizes by burning tokens.
- `transfer_`: Function to transfer tokens between addresses.
- `get_Prize_Cost`: Internal function to get the cost of a prize.
- `convert_Prize`: Internal function to convert the prize number to the corresponding enum value.
- `set_Initial_Prize_Costs`: Internal function to set the initial costs of each prize.

## Installation and Deployment
To deploy the PrizeToken contract, you can follow these steps:
1. Compile the contract using a Solidity compiler.
2. Deploy the compiled contract to an Ethereum network of your choice using tools like Remix, Truffle, or Hardhat.
3. Interact with the deployed contract using a wallet or through other smart contracts.

## License
This contract is released under the MIT License. See the SPDX-License-Identifier at the beginning of the contract file for details.

## Author

Fardeen 

fardeenmakandar99@gmail.com
