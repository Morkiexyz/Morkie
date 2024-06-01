# Morkie Platform Contracts

Morkie is a web3 application that leverages Thirdweb integration, focusing on blockchain-based interactions through smart contracts. It is designed with performance and user experience in mind.

## Smart Contracts

Our project utilizes the following smart contracts from Thirdweb:

- **OpenEditionERC721**: [Version 5.0.1](https://thirdweb.com/thirdweb.eth/OpenEditionERC721/5.0.1) - This contract allows for the creation and management of open edition NFTs, enabling users to mint and trade digital assets securely.

### Smart Contract Audits

- **OpenEditionERC721 Audit**: The audit report is available [here](https://drive.google.com/file/d/1OUD22LrEN9tq7TPBoGBqgZtrZWCrgukB/view?usp=sharing).

- **StakeERC20**: [Link to Contract](https://thirdweb.com/thirdweb.eth/TokenStake) - This contract allows users to stake their ERC-20 tokens and receive ERC-20 tokens as staking rewards (different from the staked tokens).
  - **StakeERC20 Audit**: The audit report is available [here](https://drive.google.com/file/d/1g_eFzz8EnedHrl7JdkN2hcSA_5rklQZr/view?usp=sharing).

- **StakeERC721**: [Link to Contract](https://thirdweb.com/thirdweb.eth/NFTStake) - This contract allows users to stake their ERC-721 NFTs and receive ERC-20 tokens as staking rewards.
  - **StakeERC721 Audit**: The audit report is available [here](https://drive.google.com/file/d/1g_eFzz8EnedHrl7JdkN2hcSA_5rklQZr/view?usp=sharing).

## Example: How We Call the Smart Contract

```jsx
<Web3Button
  contractAddress="0x5A3B5f1B364eF597e3E6E994810ae5f3918C7D65"
  action={async (contract) => {
    await contract.erc721.claim(value);
  }}
  onSuccess={(result) => alert("Success!")}
>
  Mint
</Web3Button>

