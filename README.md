## Vault Token (VLT)

This is a ERC20 token contract for the Vault Token (VLT).

**Features:**

* Implements the ERC20 standard for token functionalities like transfer, balance inquiry, and allowance.
* Ownable contract: Only the owner can mint new tokens.
* Burn functionality allows destroying tokens.

**Dependencies:**

    * ERC20.sol
    * Ownable.sol

**Deployment:**

1. Clone or download this repository.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Deploy the contract using your preferred development framework (e.g., Remix, Truffle, Hardhat).  

**Functions:**

* **constructor(address initialOwner)**: Initializes the token with a name ("VAULT"), symbol ("VLT"), and sets the initial owner.
* **burn(uint256 amount)**: Burns a specified amount of tokens from the message sender's address. (Only callable by an external wallet)
* **mint(address to, uint256 amount)**: Mints a specified amount of tokens to the address provided. (Restricted to owner)
* **transfer(address recipient, uint256 amount)**: Transfers a specified amount of tokens to the recipient address. (Standard ERC20 transfer function)
