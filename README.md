# MintToken

MyToken is a simpl Smart contract allows for minting and burning of tokens and keeps track of balances for each address.

## Features

1. *Public Variables:*
    - tokenName: Stores the name of the token.
    - tokenAbbrv: Stores the abbreviation of the token.
    - totalToken: Stores the total supply of the token.

2. *Mapping:*
    - balances: Maps addresses to their respective token balances.

3. *Functions:*
    - mint(address _address, uint value): Mints new tokens. Increases the total supply and the balance of the specified address.
    - burn(address _address, uint value): Burns tokens. Decreases the total supply and the balance of the specified address. Ensures that the balance of the address is sufficient to burn the specified amount.

## Usage

1. ### Minting Tokens

Call the mint function with the desired address and value. This will increase the total token supply and the balance of the given address.

```solidity
mint(address _address, uint value)
