# Video Demo 
https://youtu.be/YBk7QSzbmZM


Github: https://github.com/electrone901/intelliquiz

# IntelliQuiz

IntelliQuiz simplifies the process of creating customized quizzes on a wide range of subjects, all through straightforward inquiries. Driven by advanced AI technology, the application produces stimulating and personalized quizzes that cater to the unique interests of every user.

Once your quiz is ready, you'll be prompted to put your knowledge to the test and embark on an exciting journey of discovery. Compete against the clock, challenge your friends, and earn exciting rewards as you master each quiz. Say goodbye to mundane quizzes, and say hello to IntelliQuiz, where learning becomes an addictive and rewarding adventure! Get ready to unlock the full potential of your intellect with the ultimate quiz companion.

## How is made

- WorldCoin verifies users before they receive faucets and NFts rewards.
- ENS: Our application uses ENS to lookup ENS and fetches ENS Avatar and displays an address ENS with a Blockie image and option to copy the address.

- Mantle Testnet: The application has been deployed on the Mantle network, renowned for its secure, swift, and cost-effective transactions. We utilize this contract to meticulously record user-generated quizzes, completed quizzes, NFT awards, user profiles, and the accompanying rating systems.
  Deployed address:
  https://explorer.testnet.mantle.xyz/tx/0x2aa17b1f5212d012ba3169d548cc3558192c88d64d4f4c131d3f9ae373a2d3e3
  Tweeter:
  https://twitter.com/byBetoNY/status/1705778838507000103

- Celo Alfajores Testnet: Our application has been deployed on the Celo Alfajores Testnet, ensuring secure, rapid, and cost-effective transactions. This contract serves as the cornerstone for monitoring user-generated quizzes, successfully answered questions, NFT awards, user profiles, and the accompanying rating systems.
https://alfajores.celoscan.io/tx/0x7d3f348f3a082c2b597aa00d6ec44afee4cedd537aaa548b51459ade587da336
https://explorer.celo.org/alfajores/tx/0xcf91e68726788813b27c8176e2cae9a118aa3fc136763f0d1b91935e684bab49

- ArbitrumStylusTestnet: Arbitrum empowers our application to venture into the realm of Layer 2, enhancing scalability with rapid and cost-efficient transactions.
Deployed address arbitrumStylusTestnet 0xcAB0d540A42D7D212AdE27462721Ea86E50fA2aC
https://stylus-testnet-explorer.arbitrum.io/tx/0xf792f214ab2ec87e61234792be2645c28030bacb979b734b5ec67637eb326130

- TheGraph: We utilized the Graph to index news posts, bounties, and contributions, enabling faster sorting and retrieval of data.

- Scroll:
The application has been deployed on the Scroll network to avoid expensive transactions and to be renowned for its secure, swift, and cost-effective transactions. We utilize this contract to meticulously record user-generated quizzes, completed quizzes, NFT awards, user profiles, and the accompanying rating systems.
  Deployed address: 0x9221bde96f1EdD09716253380C8ba15C2F7d00a2
  https://sepolia-blockscout.scroll.io/tx/0xb6b05eefe578fb0979c6fbebe4a384cad6234d4ea520564d299e5f60d85a7793
  https://sepolia-blockscout.scroll.io/address/0x9221bde96f1EdD09716253380C8ba15C2F7d00a2
https://stylus-testnet-explorer.arbitrum.io/tx/0xd522ed698b7f851728dfd5af992bb0f4e18940b181145dd932c1dd3746edf0d9
https://stylus-testnet-explorer.arbitrum.io/address/0x9221bde96f1EdD09716253380C8ba15C2F7d00a2

- Mumbai Polygon Network: We deployed our dApp on the Polygon Mumbai Network with contract address 0xa766Bf75E5e8ff0F7b200AD1F1A73bEd12E11496 for secure, fastest, and unexpensive transactions. We are using this contract to keep track of the user's posted quizzes, successfully answered quizzes, NFT awards, user profiles, and rating systems. https://mumbai.polygonscan.com/address/0xa766Bf75E5e8ff0F7b200AD1F1A73bEd12E11496

- IPFS NFTStorage Used IPFS to store all food street vendor data facilitated the storage of NFTS, details of the class, and metadata of every event class. We are also, saving all the reviews, tags, class difficulty, class quality, and ratings.

- We used Solidity for the smart contract.

- We used OpenZeppelin ERC721 we use the ERC721 template for faster development of our smart contract.

- Hardhat for local blockchain development.

- We used Tailwind, MUI, Nextjs, and ReactJS for the frontend, and Ethersjs to connect to the blockchain.





## Contract Require functions
- generateQuiz function takes ipfs_url, wallet,
- mintNTFQuiz function create dynamic NFT with quiz title, my score, date, mintBlock number
  - getAllNFTs return all NFTs
  - getAllQuizzesCtreatedByMe return all quizzes

## Contents

- [Requirements](#requirements)
- [Quickstart](#quickstart)
- [Deploying your Smart Contracts to a Live Network](#deploying-your-smart-contracts-to-a-live-network)
- [Deploying your NextJS App](#deploying-your-nextjs-app)
  - [Scaffold App Configuration](#scaffold-app-configuration)
- [Interacting with your Smart Contracts: SE-2 Custom Hooks](#interacting-with-your-smart-contracts-se-2-custom-hooks)
- [Disabling Type & Linting Error Checks](#disabling-type-and-linting-error-checks)
  - [Disabling commit checks](#disabling-commit-checks)
  - [Deploying to Vercel without any checks](#deploying-to-vercel-without-any-checks)
  - [Disabling Github Workflow](#disabling-github-workflow)
- [Contributing to Scaffold-ETH 2](#contributing-to-scaffold-eth-2)

## Requirements

Before you begin, you need to install the following tools:

- [Node (v18 LTS)](https://nodejs.org/en/download/)
- Yarn ([v1](https://classic.yarnpkg.com/en/docs/install/) or [v2+](https://yarnpkg.com/getting-started/install))
- [Git](https://git-scm.com/downloads)

## Quickstart

To get started with Scaffold-ETH 2, follow the steps below:

1. Clone this repo & install dependencies

```
git clone https://github.com/scaffold-eth/scaffold-eth-2.git
cd scaffold-eth-2
yarn install
```

2. Run a local network in the first terminal:

```
yarn chain
```

This command starts a local Ethereum network using Hardhat. The network runs on your local machine and can be used for testing and development. You can customize the network configuration in `hardhat.config.ts`.

3. On a second terminal, deploy the test contract:

```
yarn deploy
```

This command deploys a test smart contract to the local network. The contract is located in `packages/hardhat/contracts` and can be modified to suit your needs. The `yarn deploy` command uses the deploy script located in `packages/hardhat/deploy` to deploy the contract to the network. You can also customize the deploy script.

4. On a third terminal, start your NextJS app:

```
yarn start
```

Visit your app on: `http://localhost:3000`. You can interact with your smart contract using the contract component or the example ui in the frontend. You can tweak the app config in `packages/nextjs/scaffold.config.ts`.

Run smart contract test with `yarn hardhat:test`

- Edit your smart contract `YourContract.sol` in `packages/hardhat/contracts`
- Edit your frontend in `packages/nextjs/pages`
- Edit your deployment scripts in `packages/hardhat/deploy`

## Deploying your Smart Contracts to a Live Network

Once you are ready to deploy your smart contracts, there are a few things you need to adjust.

1. Select the network

By default, `yarn deploy` will deploy the contract to the local network. You can change the defaultNetwork in `packages/hardhat/hardhat.config.ts.` You could also simply run `yarn deploy --network target_network` to deploy to another network.

Check the `hardhat.config.ts` for the networks that are pre-configured. You can also add other network settings to the `hardhat.config.ts` file. Here are the [Alchemy docs](https://docs.alchemy.com/docs/how-to-add-alchemy-rpc-endpoints-to-metamask) for information on specific networks.

Example: To deploy the contract to the Sepolia network, run the command below:

```
yarn deploy --network sepolia
```

2. Generate a new account or add one to deploy the contract(s) from. Additionally you will need to add your Alchemy API key. Rename `.env.example` to `.env` and fill the required keys.

```
ALCHEMY_API_KEY="",
DEPLOYER_PRIVATE_KEY=""
```

The deployer account is the account that will deploy your contracts. Additionally, the deployer account will be used to execute any function calls that are part of your deployment script.

You can generate a random account / private key with `yarn generate` or add the private key of your crypto wallet. `yarn generate` will create a random account and add the DEPLOYER_PRIVATE_KEY to the .env file. You can check the generated account with `yarn account`.

3. Deploy your smart contract(s)

Run the command below to deploy the smart contract to the target network. Make sure to have some funds in your deployer account to pay for the transaction.

```
yarn deploy --network network_name
```

4. Verify your smart contract

You can verify your smart contract on Etherscan by running:

```
yarn verify --network network_name
```

## Deploying your NextJS App

**Hint**: We recommend connecting your GitHub repo to Vercel (through the Vercel UI) so it gets automatically deployed when pushing to `main`.

If you want to deploy directly from the CLI, run `yarn vercel` and follow the steps to deploy to Vercel. Once you log in (email, github, etc), the default options should work. It'll give you a public URL.

If you want to redeploy to the same production URL you can run `yarn vercel --prod`. If you omit the `--prod` flag it will deploy it to a preview/test URL.

**Make sure to check the values of your Scaffold Configuration before deploying your NextJS App.**

### Scaffold App Configuration

You can configure different settings for your dapp at `packages/nextjs/scaffold.config.ts`.

```ts
export type ScaffoldConfig = {
  targetNetwork: chains.Chain
  pollingInterval: number
  alchemyApiKey: string
  walletConnectProjectId: string
  onlyLocalBurnerWallet: boolean
  walletAutoConnect: boolean
  // your dapp custom config, eg:
  // tokenIcon : string;
}
```

The configuration parameters are described below, make sure to update the values according to your needs:

- **targetNetwork**
  Sets the blockchain network where your dapp is deployed. Use values from `wagmi/chains`.

- **pollingInterval**
  The interval in milliseconds at which your front-end application polls the RPC servers for fresh data. _Note that this setting does not affect the local network._

- **alchemyApiKey**
  Default Alchemy API key from Scaffold ETH 2 for local testing purposes.
  It's recommended to obtain your own API key from the [Alchemy Dashboard](https://dashboard.alchemyapi.io/) and store it in an environment variable: `NEXT_PUBLIC_ALCHEMY_API_KEY` at `\packages\nextjs\.env.local` file.

- **walletConnectProjectId**
  WalletConnect's default project ID from Scaffold ETH 2 for local testing purposes.
  It's recommended to obtain your own project ID from the [WalletConnect website](https://cloud.walletconnect.com) and store it in an environment variable: `NEXT_PUBLIC_WALLET_CONNECT_PROJECT_ID` at `\packages\nextjs\.env.local` file.

- **onlyLocalBurnerWallet**
  Controls the networks where the Burner Wallet feature is available. This feature provides a lightweight wallet for users.

  - `true` => Use Burner Wallet only on hardhat network.
  - `false` => Use Burner Wallet on all networks.

- **walletAutoConnect**
  Set it to `true` to activate automatic wallet connection behavior:
  - If the user was connected into a wallet before, on page reload it reconnects automatically.
  - If user is not connected to any wallet, on reload, it connects to the burner wallet if it is enabled for the current network. See `onlyLocalBurnerWallet`

You can extend this configuration file, adding new parameters that you need to use across your dapp **(make sure you update the above type `ScaffoldConfig`)**:

```ts
  tokenIcon: "💎",
```

To use the values from the `ScaffoldConfig` in any other file of your application, you first need to import it in those files:

```ts
import scaffoldConfig from '~~/scaffold.config'
```

## Interacting with your Smart Contracts: SE-2 Custom Hooks

Scaffold-ETH 2 provides a collection of custom React hooks designed to simplify interactions with your deployed smart contracts. These hooks are wrappers around `wagmi`, automatically loading the necessary contract ABI and address. They offer an easy-to-use interface for reading from, writing to, and monitoring events emitted by your smart contracts.

To help developers get started with smart contract interaction using Scaffold-ETH 2, we've provided the following custom hooks:

- [useScaffoldContractRead](#usescaffoldcontractread): for reading public variables and getting data from read-only functions of your contract.
- [useScaffoldContractWrite](#usescaffoldcontractwrite): for sending transactions to your contract to write data or perform an action.
- [useScaffoldEventSubscriber](#usescaffoldeventsubscriber): for subscribing to your contract events and receiving real-time updates when events are emitted.
- [useScaffoldEventHistory](#usescaffoldeventhistory): for retrieving historical event logs for your contract, providing past activity data.
- [useDeployedContractInfo](#usedeployedcontractinfo): for fetching details from your contract, including the ABI and address.
- [useScaffoldContract](#usescaffoldcontract): for obtaining a contract instance that lets you interact with the methods of your deployed smart contract.

These hooks offer a simplified and streamlined interface for interacting with your smart contracts. If you need to interact with external contracts, you can use `wagmi` directly, or add external contract data to your `deployedContracts.ts` file.

### useScaffoldContractRead:

Use this hook to read public variables and get data from read-only functions of your smart contract.

```ts
const { data: totalCounter } = useScaffoldContractRead({
  contractName: 'YourContract',
  functionName: 'getGreeting',
  args: ['ARGUMENTS IF THE FUNCTION ACCEPTS ANY'],
})
```

This example retrieves the data returned by the `getGreeting` function of the `YourContract` smart contract. If the function accepts any arguments, they can be passed in the args array. The retrieved data is stored in the `data` property of the returned object.

### useScaffoldContractWrite:

Use this hook to send a transaction to your smart contract to write data or perform an action.

```ts
const { writeAsync, isLoading, isMining } = useScaffoldContractWrite({
  contractName: 'YourContract',
  functionName: 'setGreeting',
  args: ['The value to set'],
  // For payable functions, expressed in ETH
  value: '0.01',
  // The number of block confirmations to wait for before considering transaction to be confirmed (default : 1).
  blockConfirmations: 1,
  // The callback function to execute when the transaction is confirmed.
  onBlockConfirmation: (txnReceipt) => {
    console.log('Transaction blockHash', txnReceipt.blockHash)
  },
})
```

To send the transaction, you can call the `writeAsync` function returned by the hook. Here's an example usage:

```ts
<button className="btn btn-primary" onClick={writeAsync}>
  Send TX
</button>
```

This example sends a transaction to the `YourContract` smart contract to call the `setGreeting` function with the arguments passed in `args`. The `writeAsync` function sends the transaction to the smart contract, and the `isLoading` and `isMining` properties indicate whether the transaction is currently being processed by the network.

### useScaffoldEventSubscriber:

Use this hook to subscribe to events emitted by your smart contract, and receive real-time updates when these events are emitted.

```ts
useScaffoldEventSubscriber({
  contractName: 'YourContract',
  eventName: 'GreetingChange',
  // The listener function is called whenever a GreetingChange event is emitted by the contract.
  // It receives the parameters emitted by the event, for this example: GreetingChange(address greetingSetter, string newGreeting, bool premium, uint256 value);
  listener: (greetingSetter, newGreeting, premium, value) => {
    console.log(greetingSetter, newGreeting, premium, value)
  },
})
```

This example subscribes to the `GreetingChange` event emitted by the `YourContract` smart contract, and logs the parameters emitted by the event to the console whenever it is emitted. The `listener` function accepts the parameters emitted by the event, and can be customized according to your needs.

### useScaffoldEventHistory:

Use this hook to retrieve historical event logs for your smart contract, providing past activity data.

```ts
const {
  data: events,
  isLoading: isLoadingEvents,
  error: errorReadingEvents,
  } = useScaffoldEventHistory({
  contractName: "YourContract",
  eventName: "GreetingChange",
  // Specify the starting block number from which to read events, this is a bigint.
  fromBlock: 31231n,
  blockData: true,
  // Apply filters to the event based on parameter names and values { [parameterName]: value },
  filters: { premium: true }
  // If set to true it will return the transaction data for each event (default: false),
  transactionData: true,
  // If set to true it will return the receipt data for each event (default: false),
  receiptData: true
});
```

This example retrieves the historical event logs for the `GreetingChange` event of the `YourContract` smart contract, starting from block number 31231 and filtering events where the premium parameter is true. The data property of the returned object contains an array of event objects, each containing the event parameters and (optionally) the block, transaction, and receipt data. The `isLoading` property indicates whether the event logs are currently being fetched, and the `error` property contains any error that occurred during the fetching process (if applicable).

### useDeployedContractInfo:

Use this hook to fetch details about a deployed smart contract, including the ABI and address.

```ts
// ContractName: name of the deployed contract
const { data: deployedContractData } = useDeployedContractInfo(contractName)
```

This example retrieves the details of the deployed contract with the specified name and stores the details in the deployedContractData object.

### useScaffoldContract:

Use this hook to get your contract instance by providing the contract name. It enables you interact with your contract methods.
For reading data or sending transactions, it's recommended to use `useScaffoldContractRead` and `useScaffoldContractWrite`.

```ts
const { data: yourContract } = useScaffoldContract({
  contractName: 'YourContract',
})
// Returns the greeting and can be called in any function, unlike useScaffoldContractRead
await yourContract?.greeting()

// Used to write to a contract and can be called in any function
import { useWalletClient } from 'wagmi'

const { data: walletClient } = useWalletClient()
const { data: yourContract } = useScaffoldContract({
  contractName: 'YourContract',
  walletClient,
})
const setGreeting = async () => {
  // Call the method in any function
  await yourContract?.setGreeting('the greeting here')
}
```

This example uses the `useScaffoldContract` hook to obtain a contract instance for the `YourContract` smart contract. The data property of the returned object contains the contract instance that can be used to call any of the smart contract methods.

## Disabling type and linting error checks

> **Hint**
> Typescript helps you catch errors at compile time, which can save time and improve code quality, but can be challenging for those who are new to the language or who are used to the more dynamic nature of JavaScript. Below are the steps to disable type & lint check at different levels

### Disabling commit checks

We run `pre-commit` [git hook](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks) which lints the staged files and don't let you commit if there is an linting error.

To disable this, go to `.husky/pre-commit` file and comment out `yarn lint-staged --verbose`

```diff
- yarn lint-staged --verbose
+ # yarn lint-staged --verbose
```

### Deploying to Vercel without any checks

By default, Vercel runs types and lint checks before building your app. The deployment will fail if there are any types or lint errors.

To ignore these checks while deploying from the CLI, use:

```shell
yarn vercel:yolo
```

If your repo is connected to Vercel, you can set `NEXT_PUBLIC_IGNORE_BUILD_ERROR` to `true` in a [environment variable](https://vercel.com/docs/concepts/projects/environment-variables).

### Disabling Github Workflow

We have github workflow setup checkout `.github/workflows/lint.yaml` which runs types and lint error checks every time code is **pushed** to `main` branch or **pull request** is made to `main` branch

To disable it, **delete `.github` directory**

## Contributing to Scaffold-ETH 2

We welcome contributions to Scaffold-ETH 2!

Please see [CONTRIBUTING.MD](https://github.com/scaffold-eth/scaffold-eth-2/blob/main/CONTRIBUTING.md) for more information and guidelines for contributing to Scaffold-ETH 2.
