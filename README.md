This is the code for project of ETH : intermediate module 3.
In this code, I have created a ECR20 token.
@openzeppelin/contracts/token/ERC20/ERC20.sol: This imports the ERC20 standard implementation from OpenZeppelin, which provides standard functions for ERC20 tokens such as transfer, balance checking, and allowance management.
@openzeppelin/contracts/access/Ownable.sol: This imports the Ownable contract from OpenZeppelin, which allows the contract to have an owner and restrict certain functions to be callable only by the owner.
The functions used in this code are mint and burn functions.
The mint function allows the owner to mint new tokens.
The burn function allows the owner to burn his/her own tokens.
