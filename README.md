# Simple React Dapp
The frontend of this dapp is deployed at https://simple-react-dapp.netlify.app/.

The smart contract is deployed on the Sepolia Network at the address 0x5285346bF45709ECd8aB90B03135458C4fd9167B
## Instructions for deploying the contract on Sepolia Network
- Create an account on Infura and create a new project.
- Get the API key
- Get your Sepolia Account's private key from Metamask
- Copy the `.env.template` file to `.env` and fill in the `INFURA_API_KEY` and `SEPOLIA_PRIVATE_KEY` variables.
- Install dependencies with `npm install`
- Deploy the contract with `npx hardhat run scripts/deploy.js --network sepolia`. You will get the address of the deployed contract in the console.
- You can view that the contract is actually deployed on Sepolia Network by going to https://explorer.sepolia.net/ and searching for the contract address.

## Instructions for running the frontend
- Copy the address of the deployed contract and paste it in the `contractAddress` variable in the `frontend/src/App.js` file.
- `cd frontend`
- Install dependencies with `npm install`
- Run the frontend with `npm start`

## Instructions for deploying the frontend on Netlify
- Create an account on Netlify
- Connect the netlify bot to your Github account
- Create a new site from Git and select the repository of this project
- The base directory is `frontend`
- The build command is `npm install && npm run build`
- The publish directory is `frontend/build`
- Click on deploy site
