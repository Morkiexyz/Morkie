# Morkie

## Introduction

Morkie is web3 application that leveraging the power of Next.js for the frontend and Thirdweb for seamless backend integration, focusing on blockchain-based interactions through smart contracts. Designed with performance and user experience in mind, Morkie aims to provide an innovative solution in the digital art and helping artist all over the world. 

## Features

- **Next.js Frontend**: Utilizes the latest features of Next.js for fast, server-side rendered pages and optimal user experience.
- **Thirdweb Backend**: Integrates with Thirdweb for secure, scalable backend logic and blockchain interaction.
- **Blockchain Integration**: Smart contracts for minting NFTs and managing digital assets ensuring transparent and trustless transactions.

## Smart Contracts

Our project utilizes the following smart contracts

- **OpenEditionERC721**: [Version 5.0.1](https://thirdweb.com/thirdweb.eth/OpenEditionERC721/5.0.1) - This contract allows for the creation and management of open edition NFTs, enabling users to mint and trade digital assets securely.

### Smart Contract Audit

The security of the smart contracts is paramount. An independent audit was conducted to ensure their integrity and security. The audit report is available [here](https://d391b93f5f62d9c15f67142e43841acc.ipfscdn.io/ipfs/bafybeieihlxuwksuqbf55o5caopsyznu5ybvkqoxkqxtkxsqhicsmm2goq/).

## Getting Started

### Prerequisites

- Node.js
- Yarn or npm
- A wallet with [specify blockchain, e.g., Ethereum] support (e.g., MetaMask)

### How we call the Smart Contract

```jsx
<Web3Button
  contractAddress="0x5A3B5f1B364eF597e3E6E994810ae5f3918C7D65"
  action={async (contract) => {
    // Replace 'counter' with the appropriate value or logic to determine the tokenId or quantity
    await contract.erc721.claim(counter);
  }}
  onSuccess={(result) => alert("Success!")}
>
  Mint
</Web3Button>

- In case of full frontend check please dm us: morkiexyz@gmail.com

## Twitter Auth
- We use Twitter Auth 2.0 
- We dont Store any information. Twiiter auth added for user authenticity
