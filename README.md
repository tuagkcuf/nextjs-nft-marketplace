# NextJS NFT Marketplace with TheGraph

![screenshot](./public/%D0%A1%D0%BD%D0%B8%D0%BC%D0%BE%D0%BA.PNG)

## 1. Git clone the contracts repo

In it's own terminal / command line, run: 

```
git clone https://github.com/tuagkcuf/nextjs-nft-marketplace.git
cd hardhat-nextjs-nft-marketplace
yarn
```

## 2. Deploy to sepolia 

After installing dependencies, deploy your contracts to sepolia:

```
yarn hardhat deploy --network sepolia
```

## 3. Deploy your subgraph

```
cd ..
git clone https://github.com/tuagkcuf/nextjs-nft-marketplace.git
cd graph-nft-marketplace
yarn
```

Then, make a `.env` file and place your temporary query URL into it as `NEXT_PUBLIC_SUBGRAPH_URL`.


## 4. Start your UI

Make sure that:
- In your `networkMapping.json` you have an entry for `NftMarketplace` on the sepolia network. 
- You have a `NEXT_PUBLIC_SUBGRAPH_URL` in your `.env` file. 

```
yarn dev
```

