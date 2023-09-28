# Github:

https://github.com/electrone901/intelliquiz/tree/opendata

## Video

https://youtu.be/kE5oACaHRNw

# IntelliQuiz

IntelliQuiz simplifies the process of learning and creating new learning materials. With IntelliQuiz anyone can create quizzes in seconds, all powerred by AI technology, the application produces stimulating and personalized quizzes that cater to the unique interests of every user.

Once your quiz is ready, you'll be prompted to put your knowledge to the test and embark on an exciting journey of discovery. Compete against the clock, challenge your friends, and earn exciting rewards as you master each quiz. Top users will be appear on the leaderboard.

Say goodbye to mundane quizzes, and say hello to IntelliQuiz, where learning becomes an addictive and rewarding adventure! Get ready to unlock the full potential of your intellect with the ultimate quiz companion.

## How is made

# How do you use Filecoin Virtual Machine:

This application was deployed to the Filecoin Calibration testnet for its secure, swift, and cost-effective transactions. We utilize this contract to meticulously record user-generated quizzes, completed quizzes, NFT awards, user profiles, and the accompanying rating systems.
Deployed address: 0x9221bde96f1EdD09716253380C8ba15C2F7d00a2
https://calibration.filfox.info/en/address/0x9221bde96f1EdD09716253380C8ba15C2F7d00a2

# How do you use Tableland

This application makes use of tableland to
store users' quiz scores. This allows to query all scores, top 10 scores, and highest scores to display a leader board so this is a community-driven app.
-tableland stores users' NFTs info and scores: - function to store all metadata for an NFT(tx hash, quiz name, quiz id, user wallet, date) - function to store users' scores - function that returns a user scores - function that returns top 10 user scores

Deployed address: 0xB3EB0330DAADb1F7177Ef870c6Cf8abaC41A2683
https://calibration.filfox.info/en/address/0xB3EB0330DAADb1F7177Ef870c6Cf8abaC41A2683

# How do you use NFTStorage

This application is used to store metadata for NFTs rewards and metadata quiz information such as quiz description, title, category, level, language, image, author, questions, and options.

- IPFS NFTStorage Used IPFS to store all food street vendor data facilitated the storage of NFTS, details of the class, and metadata of every event class. We are also, saving all the reviews, tags, class difficulty, class quality, and ratings.

- ENS: Our application uses ENS to lookup ENS and fetches ENS Avatar and displays an address ENS with a Blockie image and option to copy the address.
- We used Solidity for the smart contract.

- We used OpenZeppelin ERC721 we use the ERC721 template for faster development of our smart contract.

- Hardhat for local blockchain development.

- We used Tailwind, MUI, Nextjs, and ReactJS for the frontend, and Ethersjs to connect to the blockchain.

## Contract Require functions

- generateQuiz function takes ipfs_url, wallet,
- mintNTFQuiz function create dynamic NFT with quiz title, my score, date, mintBlock number
  - getAllNFTs return all NFTs
  - getAllQuizzesCtreatedByMe return all quizzes

![Dashboard preview](https://raw.githubusercontent.com/electrone901/intelliquiz/881726a1612413c089377ac7023ca0b776efbdc6/2.png)
![Quiz preview](https://raw.githubusercontent.com/electrone901/intelliquiz/881726a1612413c089377ac7023ca0b776efbdc6/main.png)
![Details](https://raw.githubusercontent.com/electrone901/intelliquiz/881726a1612413c089377ac7023ca0b776efbdc6/1.png)
