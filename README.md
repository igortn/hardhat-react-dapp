## Notes

1. `npx create-react-app hardhat-react-dapp`

2. `yarn add ethers hardhat @nomiclabs/hardhat-waffle ethereum-waffle chai @nomiclabs/hardhat-ethers`

3. `npx hardhat`
    - Rename the script to `deploy.js`.
    - In the config, add the path to `artifacts` and the local hardhat network.

4. `npx hardhat compile`
    - `artifacts` get generated; `Greeter.json` contains the info that we will need for the front-end.

5. `npx hardhat node`
    - Start local network. Acccounts are generated.

6. `npx hardhat run scripts/deploy.js --network localhost`
    - Deploy the contract to the local network. Address of the contract is returned.

7. In the Metamask wallet, import account  #0 by supplying its private key.

8. React app.
   - `npm start`
   - `App.js` .
   - - Import from `react` and `ethers`. Import `Greeter.json` ABI.
   - - const `contractAddress`.  `useState()` -> `greeting`, `setGreetingValue`.
   - - Functions `fetchGreeting`,  `setGreeting`, `requestAccount`.