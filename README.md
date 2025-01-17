# ERC-20 Token

## Description
This project implements an ERC-20 token smart contract with additional functionality for retrieving transaction information. The contract was created as part of a course on blockchain technologies.

## Functionality
The contract provides the following functions:
- **`transfer`**: transfer tokens from one address to another.
- **`approve`** and **`allowance`**: allow a specific address to manage tokens.
- **`transferFrom`**: transfer tokens through a third party.
- **`balanceOf`**: get the token balance for any address.
- **`getTransactionDetails`**: returns balance information for the sender and receiver.
- **`getLatestTransactionTimestamp`**: returns the timestamp of the last transaction in `YYYY-MM-DD HH:MM:SS` format.
- **`getSenderAddress`**: Returns the sender's address.
- **`getReceiverAddress`**: Returns the receiver's address.

## Installation
1. Open the [Remix IDE](https://remix.ethereum.org/).
2. Create a new file, for example `Token.sol`, and paste the contract code.
3. Compile the contract, selecting the Solidity version 0.8.x.
4. Deploy the contract with MetaMask to one of the test networks (for example, Goerli).

## Testing
1. Use the functions in the **Deployed Contracts** section of Remix:
- **`balanceOf`**: Check the balance of addresses.
- **`transfer`**: Transfer tokens to another address.
- **`approve` and `transferFrom`**: Approve the transfer and perform it on behalf of another address.
- **`getTransactionDetails`**: Check balances after transfer.
- **`getLatestTransactionTimestamp`**, **`getSenderAddress`**, **`getReceiverAddress`**: Test helper functions.
2. Make sure values ​​are updated correctly after each transaction.

## Examples
### 1. Check balance
```solidity
balanceOf(0xYourAddress);