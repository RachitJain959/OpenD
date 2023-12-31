# OpenD NFT Marketplace

![NFT Marketplace Logo](/src/opend_assets/assets/logo.png) <!-- Replace with your logo -->

Welcome to the NFT Marketplace project on the Internet Computer! This repository contains the code for a decentralized NFT Marketplace implemented using React for the frontend and Motoko for the backend. The project enables users to mint, list, and sell NFTs on the Internet Computer platform. This document will guide you through the project, its functionalities, and how to set it up for development or deployment.

## Overview

Step into a world of boundless possibilities with our feature-rich decentralized NFT Marketplace, meticulously constructed through the synergy of React frontend elegance and Motoko backend ingenuity. Within this visionary project, users are empowered to embark on a journey of creation, commerce, and ownership, as they seamlessly mint, list, and partake in the exchange of NFTs on the revolutionary Internet Computer platform.

Picture a realm where artistic expression knows no bounds, where tokens of uniqueness and creativity take center stage. With the power to mint, users can weave their imaginative tapestries into digital form, resulting in NFTs that truly represent their essence. These digital treasures elegantly grace the marketplace, ready to be discovered, acquired, and celebrated.

Navigate to the Discover Page, an exquisite gallery where a diverse array of NFTs beckon with their allure. Engage in the art of acquisition, as you acquire the tokens of your desires by seamlessly transacting TRON tokens. With every exchange, ownership shifts, and the story of each NFT continues to unfold.

Venture to the Minter Page, a workshop of dreams, where users harness their creative energy to craft unique NFTs from their local storage. Here, digital canvases become vessels of expression, each stroke a testament to individuality. As these newly minted NFTs find their place on the "My NFTs" page, a testament to their creators' creativity emerges.

The "My NFTs" Page, a personal gallery, becomes a testament to ownership and artistic legacy. All acquired NFTs, whether procured from the captivating Discover Page or born from the depths of creativity on the Minter Page, find a home here. And as owners gaze upon their collection, they possess not only tokens of digital artistry but also the potential for trade.

Immersed within this ecosystem, transactions are seamless, powered by integrated TRON tokens. Buying and selling intertwine in a dance of commerce, and each interaction marks a step towards a more decentralized, creative future.

Welcome to a universe where technology and art converge, where tokens hold the promise of uniqueness, and where our decentralized NFT Marketplace redefines how we create, collect, and connect within the Internet Computer's innovative landscape.
## Functionalities

The NFT Marketplace project comes with the following functionalities:

1. **Discover Page**: Users can view all the listed NFTs available for sale on this page. They can purchase desired NFTs by paying the specified TRON tokens, which will be transferred to the NFT owner.

2. **Minter Page**: Users can create their own NFTs from local storage on this page. The minted NFTs will be visible on the "My NFTs" page.

3. **My NFTs Page**: Users can view all the NFTs they own, whether bought from the Discover page or minted from their local storage. They can also choose to sell their NFTs by setting the desired price in TRON tokens.

## To Install and Run the Project

1. start local dfx

```
dfx start --clean
```

2. Run NPM server

```
npm start
```

3. Deploy canisters

```
dfx deploy --argument='("CryptoDunks #123", principal ""<REPLACE WITH YOUR PRINCIPAL ID>"", (vec {137; 80; 78; 71; 13; 10; 26; 10; 0; 0; 0; 13; 73; 72; 68; 82; 0; 0; 0; 10; 0; 0; 0; 10; 8; 6; 0; 0; 0; 141; 50; 207; 189; 0; 0; 0; 1; 115; 82; 71; 66; 0; 174; 206; 28; 233; 0; 0; 0; 68; 101; 88; 73; 102; 77; 77; 0; 42; 0; 0; 0; 8; 0; 1; 135; 105; 0; 4; 0; 0; 0; 1; 0; 0; 0; 26; 0; 0; 0; 0; 0; 3; 160; 1; 0; 3; 0; 0; 0; 1; 0; 1; 0; 0; 160; 2; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 160; 3; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 0; 0; 0; 0; 59; 120; 184; 245; 0; 0; 0; 113; 73; 68; 65; 84; 24; 25; 133; 143; 203; 13; 128; 48; 12; 67; 147; 94; 97; 30; 24; 0; 198; 134; 1; 96; 30; 56; 151; 56; 212; 85; 68; 17; 88; 106; 243; 241; 235; 39; 42; 183; 114; 137; 12; 106; 73; 236; 105; 98; 227; 152; 6; 193; 42; 114; 40; 214; 126; 50; 52; 8; 74; 183; 108; 158; 159; 243; 40; 253; 186; 75; 122; 131; 64; 0; 160; 192; 168; 109; 241; 47; 244; 154; 152; 112; 237; 159; 252; 105; 64; 95; 48; 61; 12; 3; 61; 167; 244; 38; 33; 43; 148; 96; 3; 71; 8; 102; 4; 43; 140; 164; 168; 250; 23; 219; 242; 38; 84; 91; 18; 112; 63; 0; 0; 0; 0; 73; 69; 78; 68; 174; 66; 96; 130;}))'
```

4. Head to localhost

http://localhost:8080/

## Creating NFT for Testing

1. Mint an NFT on the command line to get NFT into mapOfNFTs:

```
dfx canister call opend mint '(vec {137; 80; 78; 71; 13; 10; 26; 10; 0; 0; 0; 13; 73; 72; 68; 82; 0; 0; 0; 10; 0; 0; 0; 10; 8; 6; 0; 0; 0; 141; 50; 207; 189; 0; 0; 0; 1; 115; 82; 71; 66; 0; 174; 206; 28; 233; 0; 0; 0; 68; 101; 88; 73; 102; 77; 77; 0; 42; 0; 0; 0; 8; 0; 1; 135; 105; 0; 4; 0; 0; 0; 1; 0; 0; 0; 26; 0; 0; 0; 0; 0; 3; 160; 1; 0; 3; 0; 0; 0; 1; 0; 1; 0; 0; 160; 2; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 160; 3; 0; 4; 0; 0; 0; 1; 0; 0; 0; 10; 0; 0; 0; 0; 59; 120; 184; 245; 0; 0; 0; 113; 73; 68; 65; 84; 24; 25; 133; 143; 203; 13; 128; 48; 12; 67; 147; 94; 97; 30; 24; 0; 198; 134; 1; 96; 30; 56; 151; 56; 212; 85; 68; 17; 88; 106; 243; 241; 235; 39; 42; 183; 114; 137; 12; 106; 73; 236; 105; 98; 227; 152; 6; 193; 42; 114; 40; 214; 126; 50; 52; 8; 74; 183; 108; 158; 159; 243; 40; 253; 186; 75; 122; 131; 64; 0; 160; 192; 168; 109; 241; 47; 244; 154; 152; 112; 237; 159; 252; 105; 64; 95; 48; 61; 12; 3; 61; 167; 244; 38; 33; 43; 148; 96; 3; 71; 8; 102; 4; 43; 140; 164; 168; 250; 23; 219; 242; 38; 84; 91; 18; 112; 63; 0; 0; 0; 0; 73; 69; 78; 68; 174; 66; 96; 130;}, "CryptoDunks #123")'
```

2. List the item into mapOfListings:

```
dfx canister call opend listItem '(principal "<REPLACE WITH PRINCIPAL FROM STEP1>", 2)'
```

3. Get OpenD canister ID:

```
dfx canister id opend
```

4. Transfer NFT to OpenD:

```
dfx canister call <REPLACE WITH PRINCIPAL FROM STEP1> transferOwnership '(principal "<REPLACE WITH OPEND CANISTER ID FROM STEP3>", true)'
```

## Conneting to the Token Canister

1. Copy over the token declarations folder

2. Set the token canister id into the <REPLACE WITH TOKEN CANISTER ID>

```
const TRONPrincipal = Principal.fromText("<REPLACE WITH TOKEN CANISTER ID>");
```

## Working Images

### Home

![Home Page](/src/opend_assets/images/home.png)

### Discover NFTs

![Discover Page](/src/opend_assets/images/discover.png)

### My NFTs Page

![MyNFTs Page](/src/opend_assets/images/mynfts.png)

### Create NFT

![Create Page](/src/opend_assets/images/create.png)

### Non-Listed vs Listing vs Listed NFTs for sale

![Listing](/src/opend_assets/images/listing.png)
