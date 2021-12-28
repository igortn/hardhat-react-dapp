## Notes

1. `npx create-react-app hardhat-react-dapp`

2. `yarn add ethers hardhat @nomiclabs/hardhat-waffle ethereum-waffle chai @nomiclabs/hardhat-ethers`

3. `npx hardhat`
    - Rename the script to `deploy.js`.
    - In the config, add the path to `artifacts` and the local hardhat network.

4. `npx hardhat compile`
    - `artifacts` get generated; `Greeter.json` contains the info that we will need for the front-end.
