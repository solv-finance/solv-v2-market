# solv-v2-market

Solv Voucher Market is the DeFi application for users to sell or purchase Vouchers. 

This repository contains the core smart contracts for Solv V2 Market, along with their configuration files, initialization scripts and deployment information.

More information about Solv Protocol:

- Official Website: [https://solv.finance](https://solv.finance)
- Documentation: [https://docs.solv.finance/solv-documentation](https://docs.solv.finance/solv-documentation)
- Solv Voucher Market Dapp: [https://app.solv.finance/market](https://app.solv.finance/market)

## Structure

Smart contracts are contained in the `packages` directory.

### solv-market

[`solv-market`](./packages/solv-market) is the implementation of the Solv Voucher Market. This package contains the Solv V2 Market smart contracts, configuration files and initialization scripts.


## Installation

To install Solv V2 Market, pull the repository from GitHub and to install all dependencies through `yarn` or `npm`.

```shell
git clone git@github.com:solv-finance-dev/solv-v2-market.git

cd solv-v2-market

# install with yarn
yarn install --lock-file

# or install with npm
npm install
```

## Bug Bounty

The Solv Protocol bug bounty program is focused on the smart contracts and is focused on preventing:

- Loss of user funds staked (principal) by freezing or theft
- Theft of unclaimed yield
- Freezing of unclaimed yield
- Smart contract fails to deliver promised returns

### Rewards by threat level

Rewards are distributed according to the impact of the vulnerability based on the Immunefi Vulnerability Severity Classification System.

#### Smart Contracts and Blockchain

| Threat Level | Bounty |
| :--- | :--- |
| Critical | USD $50,000 |
| High | USD $25,000 |
| Medium | USD $10,000 |
| Low | USD $3,000 |


All Critical/High severity bug reports must come with a PoC and a suggestion for a fix in order to be considered for a reward.

Payouts are handled by the Solv Protocol team directly and are denominated in USD. Payouts are done in USDT.

