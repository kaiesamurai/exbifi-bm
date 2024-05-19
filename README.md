**ExBiFi: Decentralized NFT Social Network for Curators**

**README**

**About ExBiFi:**
ExBiFi is a decentralized NFT social network designed for curators, inspired by current NFT trends and the desire for a decentralized platform. It empowers curators to earn rewards for their curation efforts by receiving a share of the proceeds when NFTs they curate are sold.

**What ExBiFi Does:**
ExBiFi transforms NFTs from static marketplace elements into dynamic assets, rewarding curators for their role in the platform. It operates as an NFT derivative exchange, with NFTs serving as the underlying assets and the value of curation staked as the NFT derivative. A quadratic formula behind the reward calculation ensures fairness by preventing users with large capital from dominating the platform.

**How It's Built:**
ExBiFi's on-chain functionality relies on the Marketplace.sol Solidity smart contract, facilitating various actions:
- Allowing users to purchase NFTs.
- Allowing curators to bond value to NFTs, represented as ERC1155 tokens minted to the curator.
- Allowing curators to claim a reward (1% of the sale) when the NFT is sold, with ERC1155 tokens representing the bonding burned to claim the reward.
ExBiFi utilizes a Chainlink External Adapter to integrate API Endpoint as a Wolfram to calculate the Curator Voting Power, determining the curator's reward entitlement. The contract is fully tested, including the Chainlink External Adapter, using the mock contracts available on Chainlink's GitHub.

For the frontend, ExBiFi employs Svelte, TailwindCSS, and Daisy UI for a user-friendly interface. Moralis API is utilized for smooth retrieval of user and NFT information.

**Challenges Faced:**
Developing a suitable formula for voting power calculation proved challenging, with Chainlink's assistance proving invaluable in optimizing gas fees. Building a fully functional service with both on-chain contracts and a polished frontend within one month was a significant accomplishment, especially considering it was the team's first collaboration.

**Accomplishments:**
Building ExBiFi from concept to reality in a short timeframe is a notable achievement. The integration of on-chain contracts with a sleek frontend UI demonstrates the team's dedication and proficiency.

**Key Learnings:**
- Complete understanding of Chainlink flow.
- Seamless integration of Moralis API for user and NFT data retrieval.
- Insights into derivative mechanics within the NFT space.

**What's Next for ExBiFi:**
The next step for ExBiFi is to launch on the Polygon Mainnet, expanding its reach and impact within the decentralized NFT ecosystem.

**Built With:**
- Blockchain (Ethereum)
- Chainlink
- DaisyUI
- Hardhat
- Moralis
- Svelte

**Try It Out:**
Explore ExBiFi's decentralized NFT social network and experience the future of curated NFT experiences.

1. Clone the repository:
   ```
   git clone 
   ```
2. Navigate to the directory and install dependencies:
   ```
   cd monorepo && npm install
   ```
3. Launch the Hardhat test:
   ```
   npx hardhat test
   ```
4. Enter the client directory and install dependencies:
   ```
   cd client && npm install
   ```
5. Run the frontend:
   ```
   npm run dev
   ```
6. Access ExBiFi at:
   ```
   http://localhost:5000
   ```

## Inspiration
ExBiFi draws inspiration from the evolving landscape of NFTs, the demand for decentralized social networks, the mechanics of traditional marketplaces, and the game theory behind derivatives. It aims to revolutionize the NFT space by creating a decentralized social network specifically tailored for curators.

## What it Does
ExBiFi transforms NFTs into dynamic assets within a social networking platform, empowering curators to earn rewards for their curation efforts. It functions as both a platform for showcasing curated NFT collections and a derivative exchange where the value of curation is staked as NFT derivatives.

## How we Built It
We developed ExBiFi using a combination of Solidity smart contracts for on-chain functionality and a frontend built with Svelte, TailwindCSS, and Daisy UI for an intuitive user experience. Chainlink was utilized for external data integration, and Moralis API facilitated smooth retrieval of user and NFT information.

## Challenges we Ran Into
One of the main challenges was devising an efficient formula for calculating curator rewards. Chainlink played a crucial role in optimizing gas fees and ensuring the scalability of the platform. Additionally, coordinating the integration of on-chain contracts with the frontend posed technical hurdles that required innovative solutions.

## Accomplishments that we're Proud of
We're proud to have built a fully functional service within a relatively short timeframe, from concept to deployment. Overcoming technical challenges and delivering a polished frontend UI while collaborating as a team for the first time demonstrates our dedication and expertise.

## What we Learned
Through the development process, we gained a deep understanding of the Chainlink flow, the seamless integration of Moralis API, and the intricacies of derivative mechanics within the NFT space. These insights will inform our future development efforts and enhance the platform's functionality.

## What's Next for ExBiFi
The next phase for ExBiFi involves launching on the Polygon Mainnet, expanding its reach and impact within the decentralized NFT ecosystem. We aim to further enhance the platform with additional features, community engagement initiatives, and partnerships to solidify its position as a leading decentralized NFT social network for curators.