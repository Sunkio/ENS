# ENS
A frontend application to showcase the ENS name of a logged-in user. The ENS (Ethereum Name Service) allows users to register and manage their ENS names.


## Getting Started
This app has been deployed to the Goerli testnet. You can access it at https://ens-gules.vercel.app/.

### Prerequisites
- [MetaMask](https://metamask.io/) installed in your browser
- [Goerli](https://goerli.net/) testnet selected in MetaMask
- [ENS](https://app.ens.domains/) name registered in MetaMask (on the goerli testnet)

## Running Locally
To run this app locally, you will need to install the following dependencies:

The frontend is built with Next.js. You need to have [Node.js](https://nodejs.org/) installed.

Run the following commands to set-up your project and start the development server:
``` shell
cd wl-frontend
rm package-lock.json
npm install
npm run dev
```
You should now be able to open the frontend in your browser on `localhost:3000`.


**Possible errors & fixes**

This project is built with node ^18. If you get an error message, you might have to update Node.js. To check your Node version, run:
``` shell
node -v
```
If you find a yarn-lock.json file, this might cause problems with installing npm in your project. Remove it and install npm again, then start your development server:
``` shell
rm yarn-lock.json
npm install
npm run dev
```

Once you’re done with the above, run:
``` shell
npm install web3modal
npm install ethers
```
Open constants/index.js and change the value of the `WHITELIST_CONTRACT_ADDRESS` variable to the address of the contract you deployed via hardhat earlier.
Then change the value of the `abi` variable to your own ABI array. You can find it here: `hardhat-tutorial/artifacts/contracts/Whitelist.sol/Whitelist.json


## How to Contribute
Contributions are always welcome! Please check the [Code of Conduct](./CODE_OF_CONDUCT.md) .

## License
This project is licensed under the [MIT License](./License.md).

## Support
If you have any questions or need help getting started, please open an issue in the repository or contact me on Twitter: @tanja_codes