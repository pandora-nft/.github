# Pandora - The NFT Lootbox

👀 Visit us here: https://pandora.on.fleek.co/

  or here: https://pandora-nft.vercel.app/

📱 Available on

- Binance Smart Chain (Testnet)
- Polygon (Testnet)
- Avalanche (Testnet)

📈 Subgraph:

- https://thegraph.com/hosted-service/subgraph/pannavich/pandora-nft-chapel
- https://thegraph.com/hosted-service/subgraph/pannavich/pandora-nft-mumbai
- https://thegraph.com/hosted-service/subgraph/pannavich/pandora-nft-fuji

# How to play with us

You can visit our deployed [website](https://pandora.on.fleek.co) and start playing around with its functionality or read more about us [here](https://github.com/pandora-nft/website/blob/main/README.md). There is also free mock nfts faucet for testing purpose in the profile/nft page.

# How to run locally

- [Requirements](#requirements)
- [Website](#website)
  - [Install Dependencies](#install-dependencies)
  - [Add Environment Variables](#add-environment-variables)
  - [Start Developing](#start-developing)
- [Get Mock NFTs](#get-mock-nfts)
  - [Add Environment Variables](#add-environment-variables-1)
  - [Run Scripts](#run-scripts)
    - [Get Mock NFTs](#get-mock-nfts)

# Requirements

```
- yarn
- hardhat
- solidity
```

# Website

Go to website repository [here](https://github.com/pandora-nft/website) and clone to your local machine

## Install Dependencies

    yarn

## Add Environment Variables

You need to add your environment variables to the
`.env.local` file:

```
NEXT_PUBLIC_MORALIS_SERVER_URL=https://xxxxxxxx.usemoralis.com:2053/server
NEXT_PUBLIC_MORALIS_APP_ID=abdsafasfcasFADSFSAFAgkfldsgj
NEXT_PUBLIC_BSCTESTNET_RPC_URL=https://speedy-nodes-nyc.moralis.io/<YOUR_NODE_ID>/bsc/testnet
NEXT_PUBLIC_MUMBAI_RPC_URL=https://speedy-nodes-nyc.moralis.io/<YOUR_NODE_ID>/polygon/mumbai
NEXT_PUBLIC_FUJI_RPC_URL=https://speedy-nodes-nyc.moralis.io/<YOUR_NODE_ID>/avalanche/testnet
```

## Start Developing

    yarn dev

then visit http://localhost:3000/

# Smart contracts

Go to contracts repository [here](https://github.com/pandora-nft/contracts) and clone to your local machine

## Add Environment Variables

You need to add your environment variables to the `.env` file,

    PRIVATE_KEY=

    MUMBAI_URL=
    BSC_TESTNET_URL=
    FUJI_URL=

    POLYGONSCAN_API_KEY=
    BSCSCAN_API_KEY=
    SNOWTRACE_API_KEY=

The must add is PRIVATE_KEY for signing the smartcontract.
and the `RPC URL` of your choice, otherwise you can easily get all of them by register with [Moralis](https://moralis.io/) and get the speedy nodes.

The XXX_API_KEY is for verifying smartcontract deployment.

## Run Scripts

### Get Mock NFTs

    yarn hardhat run scripts/getMockNFT.ts --network <NETWORK_OF_YOUR_CHOICE>

You will get mock nfts, and now you are ready to play with the Pandora NFT Lootbox 🎉
