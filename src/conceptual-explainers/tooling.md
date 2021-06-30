# Tooling

## CKB Node

Nervos Network is a decentralized and permissionless multi-layer blockchain ecosystem. The Nervos blockchain, also known as the Common Knowledge Base, is the bottom-most layer in the Nervos ecosystem. It serves as a foundation to build on and provides trust to all layers built on top. It is designed to maximize decentralization while remaining minimal, flexible, and secure. Its main purpose is the reliable preservation of any data and assets stored within it.

The focus of layer 1 is security and decentralization. Layer 1 provides a source of trust to all layers above it. Layer 2 focuses on scalability, providing high-throughput with millions of transactions per second. The two layers function together to achieve higher levels of decentralization, security, and scalability than are possible on a single layer.

The CKB node software is what powers the layer 1 blockchain. It handles the aspects of networking, consensus, smart contract execution, data storage, and data retrieval. CKB nodes are run by all participants of the network that need RPC access to the information contained within the blockchain.

- [Github](https://github.com/nervosnetwork/ckb)
- [Download](https://github.com/nervosnetwork/ckb/releases)
- Setup Guides for [[Mainnet](https://docs.nervos.org/docs/basics/guides/mainnet)] [[Testnet](https://docs.nervos.org/docs/basics/guides/testnet)] [[Devnet](https://docs.nervos.org/docs/basics/guides/devchain)] [[Docker](https://docs.nervos.org/docs/basics/guides/run-ckb-with-docker)]
- [CKB JSON-RPC Guide](https://docs.nervos.org/docs/reference/rpc)
- [CKB JSON-RPC Documentation](https://github.com/nervosnetwork/ckb/blob/master/rpc/README.md)

## CKB Indexer

The CKB Indexer handles the organization (indexing) of specific pieces of blockchain data which are commonly needed for dapp development. The CKB Indexer runs besides the CKB node software to add additional functionality for developers that is not required by the CKB node software for consensus.

In some other blockchain node software, the functionality of the indexer included with the main node software. However, this adds a significant amount of overhead to both the disk space requirements and the processing of each block. This, in turn, increases the resources required to run a basic node on the network.

Nervos splits this functionality into two distinctly different pieces of software. This keeps the system requirements of the CKB node software at a bare minimum, which reduces the burden necessary to run a full node, and allows more people to run one to encourage higher levels of decentralization. Developers can optionally install the CKB Indexer when they require more functionality.

- [Github](https://github.com/nervosnetwork/ckb-indexer)
- [Download](https://github.com/nervosnetwork/ckb-indexer/releases)
- [Basic Usage Instructions](https://github.com/nervosnetwork/ckb-indexer/blob/master/README.md)

## CKB-CLI

CKB-CLI is a command line tool that is used with a CKB node to perform common actions such as creating accounts, sending CKBytes, and querying the blockchain for transaction data.

CKB-CLI can be downloaded separately, but it is also included with the native CKB node software.

- [Github](https://github.com/nervosnetwork/ckb-cli)
- [Download](https://github.com/nervosnetwork/ckb-cli/releases)
- [Documentation](https://github.com/nervosnetwork/ckb-cli/blob/develop/README.md)

## Tippy

Tippy is a tool for managing instances of CKB nodes and CKB Indexers using a desktop GUI interface. Tippy allows you to create Mainnet, Testnet, and Devnet chains with just a few clicks.

Tippy is very useful for developers to manage multiple Devnet chains quickly without having spend time moving data around on the command line.

- [Github](https://github.com/nervosnetwork/tippy)
- [Download](https://github.com/nervosnetwork/tippy/releases)
- [Documentation](https://github.com/nervosnetwork/tippy/blob/develop/README.md)

## Thunder Issue SUDT

Thunder Issue SUDT is a dapp to manage the creation of SUDT tokens and token meta data. An SUDT token stands for Simple User Defined Token. This is the Nervos equivalent of the Ethereum ERC20 standard, which allows for the creation of basic common tokens.

Thunder Issue SUDT relies on the [Keypering](https://nervosnetwork.github.io/keypering/) wallet for all actions.

- [Official Website](https://udt.ckbapp.dev/)
- [Github](https://github.com/zmcNotafraid/thunder-issue-SUDT)

## CKB.tools

CKB.tools is a online collection of free development tools created for use with Nervos Network.

The current tools available include:

- Address Tool - A tool to view the components and attributes of Nervos CKB addresses.
- Bootstrap - Recent snapshots of the Testnet chain data to speed up the initial sync.
- SUDT Tool - A tool to create SUDT tokens on the Testnet using MetaMask.

All tools rely on the MetaMask wallet exclusively, and run completely in the browser. No other dependencies are needed.

- [Official Website](https://ckb.tools/)
- [Github](https://github.com/jordanmack/ckb-tools)