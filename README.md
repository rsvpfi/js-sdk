# Streamflow

Streamflow is a token vesting and streaming payments platform.

There are several ways to use **Streamflow**:

- **(easiest) [app.streamflow.finance](https://app.streamflow.finance?utm_medium=github.com&utm_source=referral&utm_campaign=js-sdk-repo)** (React application that uses JS SDK directly)
- **[JS SDK](https://github.com/streamflow-finance/js-sdk)** to interact with the protocol => [NPM package](https://www.npmjs.com/package/@streamflow/stream)
- **[Rust SDK](https://github.com/streamflow-finance/rust-sdk)** to integrate within a Solana program => [Rust Crate](https://docs.rs/streamflow-sdk/)

**Security audit passed ✅**

Protocol audits available [here](https://www.notion.so/streamflow/Streamflow-Security-Audits-3250070c0b3a4a0690385d96316d645c).  
Partner oracle audit available [here](https://github.com/streamflow-finance/rust-sdk/blob/main/partner_oracle_audit.pdf).

## Documentation
API Documentation available here: [docs site →](https://js-sdk-docs.streamflow.finance/)

## JS SDK to interact with Streamflow protocols

This repo consists of js-sdk to interact with several protocol exposed by streamflow:
- `packages/stream` - [Core Streamflow Protocol](packages/stream/README.md) that allows to create a vesting/payment/lock Stream to a Recipient;
- `packages/distributor` - [Distributor Streamflow Protocol](packages/distributor/README.md) that allows to Airdrop tokens to large amount of Recipients (thousands or even millions);
- `packages/common` - Common utilities and types used by Streamflow SDK;

## Installation

### Install Stream Protocol SDK

```bash
npm i -s @streamflow/stream
# or
yarn add @streamflow/stream
```

### Install Distributor Protocol SDK

```bash
npm i -s @streamflow/common @streamflow/distributor
# or
yarn add @streamflow/common @streamflow/distributor
```

## Environments
For web browser runtimes polyfills might be required. SDKs use `node:` prefixed modules, for instance: `node:crypto`. However, transitive 3rd parties might use non-prefixed modules so both ways of importing should be polyfilled.

The easiest way to achieve it is using a bundler's plugin.
For polyfills take a look on these libraries:
1. Vite - https://www.npmjs.com/package/vite-plugin-node-polyfills
2. Rsbuild - https://github.com/rspack-contrib/rsbuild-plugin-node-polyfill
3. Webpack - https://www.npmjs.com/package/node-polyfill-webpack-plugin

## Contributing

To contribute to this repository, please follow these steps:

1. Fork the repository
2. Clone your forked repository
3. Navigate to the `/packages` folder
4. Install dependencies using pnpm:
   ```bash
   pnpm install
   ```
5. Build the project:
   ```bash
   pnpm build
   ```
6. Make your changes
7. Commit and push your changes
8. Create a pull request

Please ensure that you have [pnpm](https://pnpm.io/) installed on your system before contributing.

## News
Stay updated on our [X/Twitter](https://x.com/streamflow_fi).

<!-- commit on 2025-01-21 -->

<!-- commit on 2025-02-21 -->

<!-- commit on 2025-02-04 -->

<!-- commit on 2025-02-06 -->
