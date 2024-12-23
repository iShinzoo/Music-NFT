# MusicBlock NFT Smart Contract

## Overview

MusicBlock is an ERC-721 compliant NFT smart contract built using Solidity. The contract allows users to mint unique MusicBlock NFTs with metadata stored on IPFS. It leverages OpenZeppelin’s libraries for security and standardized functionality.

## Features

* ERC-721 Compliance: Implements the ERC-721 standard for non-fungible tokens.

* Token URI Storage: Supports custom metadata for each token using the ERC721URIStorage extension.

* IPFS Integration: Base URI is set to point to IPFS for decentralized metadata storage.

* Safe Minting: Ensures tokens are securely minted to the user's wallet.

*** Checkout NFT from here 👇***

[Click Me !](https://testnets.opensea.io/collection/musicblock-8)

## Prerequisites

* Node.js: Required for interacting with Ethereum blockchain.

* Hardhat: For local development and testing.

* MetaMask: Wallet for interacting with the contract on supported networks.

* IPFS: For hosting metadata files.

## Technologies Used

* Solidity (v0.8.22): Smart contract programming language.

* OpenZeppelin: Industry-standard library for secure and modular smart contracts.

* Ethereum: Blockchain for deploying and interacting with the smart contract.

## Contract Details

### Contract Name

* MusicNFT

### Symbol

* MBC

## Functions

* mintNFT() -
   Mints a new NFT to the caller's address.
   Automatically increments the token ID for each new token.

* _baseURI() -
  Returns the base URI for token metadata.
  Overridden to provide a custom base URI.

* tokenURI(uint256 tokenId) -
  Returns the metadata URI for a specific token ID.
  Ensures the token exists before providing the URI.

## Dependencies

```
@openzeppelin/contracts/token/ERC721/ERC721.sol
@openzeppelin/contracts/token/ERC721/extensions/ERC721URIStorage.sol
@openzeppelin/contracts/utils/Counters.sol
```

## Setup and Deployment

Step 1: Clone the Repository
```
git clone <repository-url>
cd <repository-folder>
```

Step 2: Install Dependencies
```
npm install
```

Step 3: Compile the Contract
```
npx hardhat compile
```

Step 4: Deploy the Contract

Update the deployment script with your desired network configuration.

Deploy the contract:
```
npx hardhat run scripts/deploy.js --network <network-name>
```

Step 5: Interact with the Contract

Use a tool like Hardhat Console or Ethers.js to interact with the deployed contract. Example:
```
const contract = await ethers.getContractAt("MusicNFT", "<contract-address>");
await contract.mintNFT();
```

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments

* OpenZeppelin Contracts

* Hardhat

## Contact

For questions or support, please contact:

Email: work.krsna4@gmail.com

