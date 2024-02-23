
SimpleToken Contract README
Overview:-
The SimpleToken contract is a basic implementation of a token on the Ethereum blockchain. It follows the ERC-20 standard, providing functionalities for token creation, transfer, and destruction. The contract is written in Solidity, a programming language specifically designed for smart contracts on the Ethereum platform.

License:-
This smart contract is licensed under the MIT License. Please refer to the SPDX-License-Identifier and the license text within the source code for more details.

Contract Details:-
Public Variables:-
tokenName: A string representing the name of the token.
tokenAbbrv: A string representing the abbreviation or symbol of the token.
totalSupply: An unsigned integer representing the total supply of the token.
Mapping
balances: A mapping from Ethereum addresses to their corresponding token balances.
Events
Mint: An event emitted when new tokens are minted. It logs the recipient's address and the minted value.
Burn: An event emitted when tokens are burned (destroyed). It logs the sender's address and the burned value.
Constructor
Initializes the token with a name, abbreviation, and initial supply.
Assigns the initial supply to the address deploying the contract.
Functions
mint(address _to, uint256 _value): Creates new tokens and assigns them to the specified address.
burn(address _from, uint256 _value): Destroys tokens from the specified address.
Usage
Deploy the SimpleToken contract on the Ethereum blockchain.
Use the constructor to set the token name, abbreviation, and initial supply.
Interact with the contract through the mint and burn functions to manage token supply.



Example:-
// Deploy the contract with name "MyToken", abbreviation "MT", and initial supply of 1000 tokens
SimpleToken myToken = new SimpleToken("MyToken", "MT", 1000);

// Mint 500 tokens to address 0x123
myToken.mint(0x123, 500);

// Burn 200 tokens from address 0x456
myToken.burn(0x456, 200);

Note:-
This is a simple example and may not cover all aspects of a production-ready token contract.
Ensure you understand the implications of minting and burning tokens, as well as the security considerations for deploying contracts on the Ethereum blockchain.
Always review and test the code thoroughly before deploying it on the mainnet.
