# ERC20 and Vault Contracts

## ERC20 Contract

The ERC20 contract provides a standard interface for fungible tokens on the Ethereum blockchain. It includes functionalities such as transferring tokens between addresses, approving spending on behalf of another address, and allowing token allowance management.

### Features:
- **Token Transfer**: Users can transfer tokens from their account to another Ethereum address.
- **Token Approval**: Users can approve another Ethereum address to spend tokens on their behalf.
- **Token Transfer From**: Allows approved addresses to transfer tokens on behalf of the token owner.
- **Token Minting**: Token owners can create new tokens, increasing the total token supply.
- **Token Burning**: Token owners can destroy tokens, decreasing the total token supply.

### Events:
- **Transfer**: Triggered whenever tokens are transferred between addresses.
- **Approval**: Triggered when token approval is granted for spending.

## Vault Contract

The Vault contract serves as a secure storage solution for ERC20 tokens, allowing users to deposit and withdraw tokens while minting and burning corresponding "shares" within the vault. It implements the ERC20 interface for seamless interaction with ERC20 tokens.

### Features:
- **Deposit**: Users can deposit ERC20 tokens into the vault, receiving "shares" equivalent to their deposited amount.
- **Withdraw**: Users can withdraw tokens from the vault by burning their "shares," receiving the corresponding amount of ERC20 tokens.
- **Shares Management**: Tracks the total supply of shares and individual share balances for users.
- **Efficient Deposits and Withdrawals**: Computes shares dynamically to ensure fair token distribution upon deposit and withdrawal.

### Events:
- No additional events defined within the Vault contract.

## Usage Instructions:

1. **Deploy Contracts**: Deploy both the ERC20 and Vault contracts to the Ethereum blockchain.
2. **Interact with ERC20**: Use the ERC20 contract to mint tokens, transfer tokens, or burn tokens as needed.
3. **Interact with Vault**: Deposit ERC20 tokens into the Vault contract to receive shares, and withdraw tokens by burning shares.

## Auhtor

Sunil KS
