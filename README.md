# POAP EX

POAP EX is a contract wallet that fills the gap in the POAP ecosystem, enhancing the POAP economic system to perfection. It enables the binding of any asset, such as NFTs or ERC20 tokens, to a POAP token by leveraging the sponsor tech.

## Introduction

POAP EX is the final puzzle piece, ingeniously filling the gap in the POAP ecosystem and bringing the POAP economic system to its ultimate perfection

POAP EX is a contract wallet that allows POAP (Proof of Attendance Protocol) to bind any asset, such as NFTs or ERC20 tokens, to a POAP token. It leverages the sponsor tech to enable this functionality.

By utilizing the ERC6551 Contract Wallet proposal, POAP EX creates a contract wallet specifically for POAP tokens. This contract wallet acts as a smart contract account associated with each POAP token, granting it the ability to own and manage assets. With this integration, POAP EX allows users to bind additional assets (such as NFTs or ERC20 tokens) to their POAP tokens, making it easier to organize and control various assets associated with events and participation.

Before the introduction of POAP EX, users might have had multiple POAP tokens and other assets scattered across different wallets, making it challenging to manage and keep track of them. However, by implementing the ERC6551 Contract Wallet proposal, POAP EX offers a solution by creating a contract wallet specifically for POAP tokens. This contract wallet acts as a centralized hub, allowing users to control and manage their POAP tokens along with associated assets, providing a more streamlined and organized experience.

In addition to improved asset management, the sponsor tech integration with POAP EX enables various use cases such as access control, loyalty cards, and GameFi starter kits. For example, the contract wallet can be used for granting permissions, allowing users to access specific resources or features within the context of the ERC6551 Contract Wallet. It can also function as a loyalty card, where users can utilize ERC-4337 to redeem points without incurring gas fees. GameFi projects can leverage POAP EX to store game assets as starter kits and distribute them in the form of POAP tokens during events.

Overall, by utilizing the sponsor tech and the ERC6551 Contract Wallet proposal, POAP EX enhances the functionality and utility of POAP tokens, allowing for a more comprehensive and integrated asset management solution while enabling various use cases within the ecosystem.

## What we have built?

Based on our discussion, here is a detailed description of the features and functionality that POAP EX has built-in:

1. Contract Wallet Creation: POAP EX facilitates the creation of a contract wallet specifically designed for POAP tokens. This contract wallet acts as a centralized hub for managing and controlling POAP tokens and associated assets.

2. Asset Binding: POAP EX allows users to bind additional assets to their POAP tokens. These assets can include NFTs (non-fungible tokens) and ERC20 tokens. By binding assets to POAP tokens, users can conveniently manage and access all their assets from within the POAP ecosystem.

3. Streamlined Asset Management: With POAP EX, users no longer need to manage multiple wallets or scattered assets. The contract wallet provides a centralized location where users can organize and control their POAP tokens and associated assets, making asset management more streamlined and efficient.

4. Access Control: POAP EX leverages the ERC6551 Contract Wallet proposal to enable granular access control. Users can grant permissions to specific resources or features within the context of the contract wallet. This allows for a customizable approach to access control, tailoring it to the specific needs of different use cases.

5. Loyalty Card Functionality: The contract wallet can also function as a loyalty card. POAP EX integrates ERC-4337, which allows users to redeem loyalty points without incurring gas fees. This feature enhances the usability of POAP tokens as a loyalty program within applications.

6. GameFi Starter Kit: POAP EX caters to GameFi projects by enabling the storage and distribution of various game assets as starter kits. These assets can be distributed in the form of POAP tokens during events or as rewards, enhancing user engagement and incentivizing participation.

By incorporating these features, POAP EX provides a comprehensive solution for asset management and utilization within the POAP ecosystem. It enhances the functionality of POAP tokens, allowing users to control their assets more effectively, while enabling access control, loyalty card functionality, and catering to GameFi projects' specific needs.

## Features

- Contract Wallet Creation: POAP EX facilitates the creation of a contract wallet specifically designed for POAP tokens, allowing centralized management and control of POAP tokens and associated assets.
- Asset Binding: Users can bind additional assets, including NFTs and ERC20 tokens, to their POAP tokens within the contract wallet, providing streamlined asset management.
- Access Control: Granular permissions can be granted within the contract wallet, allowing customizable access control for specific resources or features.
- Loyalty Card Functionality: The contract wallet acts as a loyalty card, integrating ERC-4337 for gas-free redemption of loyalty points using POAP tokens.
- GameFi Starter Kit: POAP EX supports GameFi projects by enabling storage and distribution of game assets as starter kits in the form of POAP tokens.

## Contracts

- [ERC6551Registry](https://gnosisscan.io/address/0x49ca22a4cb2de5e8ec1edcbae9092c4971b8b957)
- [Account Implementation](https://gnosisscan.io/address/0x82aC997d69f2649bBD3B0FEfcAe800edC1aAcD67)
- [Sample ERC6551 Account](https://gnosisscan.io/address/0xb49090f95fe0f92f9e10d202c399a36f7951c9e7)

## Demo

- [Demo Video](https://www.youtube.com/watch?v=iWA9wV9d83Q&ab_channel=%E8%AC%9D%E5%BF%A0%E7%A9%8E)
- [Demo Site](https://erc6551-gnosis.vercel.app/)
- [Presentation](https://gamma.app/docs/POAP-EXHackathon-of-Web3-POAP-r46kwmu1oas75am?mode=doc)

## Usage

### Contracts

```bash
# Build and test
forge build
forge test

# Deploy ERC6551Registry
forge create --rpc-url $RPC_URL --private-key $PRIVATE_KEY src/ERC6551Registry.sol:ERC6551Registry

# Deploy ExampleERC6551Account
forge create --rpc-url $RPC_URL --private-key $PRIVATE_KEY src/ExampleERC6551Account.sol:ExampleERC6551Account

# Create account using ERC6551Registry
cast send --value 0 --rpc-url $RPC_URL --chain 100 --etherscan-api-key $GNOSISSCAN_API_KEY --private-key $PRIVATE_KEY $REGISTRY_ADDRESS "createAccount(address,uint256,address,uint256,uint256,bytes)" $IMPLEMENTATION_ADDRESS 100 $CONTRACT_ADDRESS $TOKEN_ID 0 ""
```

### Frontend

```bash
pnpm install
pnpm run dev
```

Please refer to the GitHub repository for detailed documentation and instructions.

## License

This project is licensed under the terms of the MIT License. See the [LICENSE](https://chat.openai.com/c/LICENSE) file for details.
Feel free to customize and add additional sections based on the specific needs and nature of your project.
