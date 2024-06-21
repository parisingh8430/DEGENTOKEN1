The DegenToken contract is implemented in Solidity version 0.8. It inherits from the IERC20 interface, providing standard ERC20 functionality. The contract has the following features:

Token name: DegenToken
Token symbol: DGN

totalSupply(): Returns the total supply of DegenTokens.
balanceOf(address account): Returns the token balance of the specified account.
transfer(address to, uint256 value): Transfers tokens from the sender's account to the specified recipient.
burn(uint256 value): Burns tokens from the sender's account, reducing the total supply.
mint(address to, uint256 value): Mints new tokens and assigns them to the specified recipient. Only the contract owner can perform this operation.
getPurchases(address account): Retrieves the list of purchases made by the specified account.
redeem(string memory itemName, uint256 value): Allows the sender to redeem tokens for an item in the in-game store.
allowance(address owner, address spender): Returns the amount of tokens that the spender is allowed to spend on behalf of the owner.
approve(address spender, uint256 value): Approves the spender to transfer a specific amount of tokens from the sender's account.
transferFrom(address from, address to, uint256 value): Transfers tokens from one address to another on behalf of a specified address.


Install the project dependencies: npm install
Set up your Avalanche network provider and account credentials in the Hardhat configuration file(hardaht.config.js).
Deploy the contract to the Avalanche network using Hardhat: npx hardhat run scripts/deploy.js --network fuji 
Interact with the deployed contract by using remix.
