MyToken - ERC20 Token Contract
Overview
This project is part of the ETH Intermediate Module 3. MyToken is an ERC20 token contract implemented in Solidity. It leverages OpenZeppelin's ERC20 and Ownable contracts to ensure security and functionality. The contract allows the owner to mint new tokens and any token holder to burn their tokens.

Features
Minting: The owner of the contract can mint new tokens to any specified address.
Burning: Token holders have the ability to burn their own tokens, reducing the total supply.
Prerequisites
Before you begin, ensure you have met the following requirements:

Node.js and npm: These are required to install dependencies and run the project.
Truffle or Hardhat: Choose either of these frameworks for smart contract development.
OpenZeppelin Contracts: This library provides secure and standardized implementations of ERC20 and Ownable contracts.
Only the contract owner can mint new tokens. Use the following function to mint tokens:function mint(address to, uint256 amount) public onlyOwner {
    _mint(to, amount);
}
Any token holder can burn their own tokens. Use the following function to burn tokens:function burn(uint256 amount) public {
    _burn(msg.sender, amount);
}

