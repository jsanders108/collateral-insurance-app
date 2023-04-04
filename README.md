This is a full-stack Solidity collateral insurance app (using Ethers.js). A customer may purchase insurance for collateral used to secure a crypto loan and be covered for up to 30 ETH in case of liquidation. There are 2 policy types: 

  1) For 0.04 ETH, a customer may purchase 100% coverage for up to 30 ETH for 60 days.
  2) For 0.02 ETH, a customer may purchase 75% coverage for up to 30 ETH for 60 days. 

This app's smart contracts are currently deployed on the Polygon Mumbai testnet (due to high gas fees on the Goerli ETH testnet). The app employs the "factory" method: when a customer purchases a new insurance policy, a new smart contract for that specific policy is created and deployed each time by the "Collateral Policy Factory Contract". 

The "Collateral Depository" smart contract holds all the funds deposited by customers when purchasing their insurance policies. The Collateral Depository pays out claims that are approved by the administrator. It is also possible for the administrator to deposit funds into the Compound Finance defi protocol (and get cETH tokens in return) to earn a yield (this functionality will be possible when deployed to Goerli or mainnet Ethereum). 

Here is the contract address for the Collateral Depository: 0x9901a3Be929fC71aBbb5F3A33746c968299F55Df  (Polygon Mumbai testnet)

Here is the contract address for the Collateral Policy Factory: 0x7366B655E075826AbF75972FCfAe5180149c37c4 (Polygon Mumbai testnet)

The app can be accessed at the following website: https://collateral-insurance-app.netlify.app/
