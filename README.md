# Project Title
MyToken

# Solidity
A simple ERC-20 token contract Written in Solidity for creating and managing tokens on a Blockchain.
REQUIREMENTS
    1. Your contract will have public variables that store the details about your coin (Token Name, Token Abbrv., Total Supply)
    2. Your contract will have a mapping of addresses to balances (address => uint)
    3. You will have a mint function that takes two parameters: an address and a value. 
       The function then increases the total supply by that number and increases the balance 
       of the “sender” address by that amount
    4. Your contract will have a burn function, which works the opposite of the mint function, as it will destroy tokens. 
       It will take an address and value just like the mint functions. It will then deduct the value from the total supply 
       and from the balance of the “sender”.
    5. Lastly, your burn function should have conditionals to make sure the balance of "sender" is greater than or equal 
       to the amount that is supposed to be burned.

# How to run the program
1.Compile 'MyToken.sol' using the Remix IDE or the Solidity compiler ('solc'). Verify that Solidity version '0.8.18' is compatible.
2.Select a deployment environment (e.g., Ethereum mainnet, Rinkeby testnet, or the JavaScript VM in the Remix IDE).
Install the MyToken contract. It starts with the values tokenName = "Bitcoin", tokenAbbrv = "BTC", and totalSupply = 0.
3.To communicate with deployed contracts, use MetaMask or another Ethereum wallet.
Utilize features like mint and burn to control the quantity and balance of tokens.
4. Minting Tokens:
   - Call `mint(address _address, uint _value)` function:
     - Provide `_address` to mint tokens to.
     - Specify `_value` (amount of tokens) to mint.
     - Update `totalSupply` and `_address`'s balance accordingly.
5.Burning Tokens:
   - Call `burn(address _address, uint _value)` function:
     - Ensure `_address` has sufficient tokens (`balances[_address] >= _value`).
     - Burn `_value` tokens from `_address`.
     - Decrease `totalSupply` and `_address`'s balance accordingly.
6.Gas fees for transactions (minting/burning) must be paid in ETH.
Use wallet APIs or the Remix IDE to estimate gas expenses.
Keep an eye on your ETH balance to make sure you have enough money for transactions.
7.Security considerations: - Use access restrictions to limit the functionality of `mint` and `burn` if necessary.
   - For input validation (e.g., sufficient balances), use `require` statements.
   - Use secure wallets (MetaMask, hardware wallets) and take precautions with private keys.
8.Before releasing on the Ethereum mainnet, extensively evaluate the functioning of the contract on testnets.
To debug contract interactions, use the logging events feature in Remix IDE or the debugger.
9.Include tokenomics and function information in the contract specs.
Maintaining adherence to ERC20 standards is essential for increased interoperability and compatibility.


# Description
Bitcoin is a basic implementation of an ERC-20 token contract ,allowing users to mint and burn tokens.The contract stores token balances in a mapping and updates the total supply accordingly.This contract can be used as a starting point for more complex token implementations.

# Author
Vemula Narendra 
