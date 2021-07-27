# solv-market

`solv-market` contains the Solv V2 Market smart contracts, configuration files, initialization scripts and testcases.


## Contracts

- [SolvICMarket](./contracts/SolvICMarket.sol)

	- `SolvICMarket` is the core smart contract of the Solv Voucher Market, which provides extries for users to publish orders at fixed/declining prices, cancel target orders, or purchase Vouchers by units/payment amount.

- [PriceManager](./contracts/PriceManager.sol)

	- `PriceManager` is a util contract allowing users to set fixed/declining prices for a Voucher order, or query price of any Voucher order. 

## Deploy, Initialize and Test

### Deployment

```shell
cd solv-market
yarn compile

# for local deployment, run:
yarn deploy:localhost

# for deployment with target network(see: hardhat.config.ts), run:
yarn deploy --network `network`
```

### Initialization

- Set solver address (required) (`Solver` should have been deployed, see: [solv-v2-voucher](git@github.com:solv-finance-dev/solv-v2-voucher.git))

```shell
# see hardhat.config.ts for network configuration
npx hardhat test init/init-impl.ts --network `network`
```

- Add markets (optional) (target Vouchers should have been deployed, see: [solv-v2-voucher](git@github.com:solv-finance-dev/solv-v2-voucher.git))

```shell
# see hardhat.config.ts for network configuration
npx hardhat test init/add-market.ts --network `network`
```

- Add payment currencies (optional)

```shell
# see hardhat.config.ts for network configuration
npx hardhat test init/add-currencies.ts --network `network`
```

### Test

```shell
# for local deployment, run:
yarn test:localhost

# for deployment with target network(see: hardhat.config.ts), run:
yarn test --network `network`
```


