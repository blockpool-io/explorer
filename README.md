# Blockpool Explorer 3.0

<p align="center">
    <img src="/banner.png" />
</p>

> Designed and developed from the ground-up, using lean & fast developmental frameworks (Tailwind CSS & Vue.JS).

[![Build Status](https://badgen.now.sh/circleci/github/blockpool-io/explorer-3.0)](https://circleci.com/gh/blockpool-io/explorer-3.0)
[![Codecov](https://badgen.now.sh/codecov/c/github/blockpool-io/explorer-3.0)](https://codecov.io/gh/blockpool-io/explorer-3.0)
[![License: MIT](https://badgen.now.sh/badge/license/MIT/green)](https://opensource.org/licenses/MIT)

> Lead Maintainer: [Michel Kraaijeveld](https://github.com/ItsANameToo)

You can access it at [https://explorer.blockpool.io/](https://explorer.blockpool.io/).

## Build Setup

### 1. Clone the repository

```bash
git clone https://github.com/blockpool-io/explorer-3.0
```

### 2. Install Dependencies

```bash
yarn install
```

### 3. Build for Production

#### 3.1 Mainnet

```bash
yarn build:mainnet
```

#### 3.2 Devnet

```bash
yarn build:devnet
```

#### 3.3 Custom

```bash
yarn build --network my-custom-network
```

#### 3.5 Run Express Server

You can run the explorer as an express server. This makes it a little more light-weight but not needing to have services such as apache or nginx.

```bash
EXPLORER_HOST="127.0.0.1" EXPLORER_PORT="4200" node express-server.js
```

> Keep in mind that this requires you to run your own server and a running instance of nginx.

### 4. Development

#### 4.1 Mainnet

```bash
yarn dev # or yarn dev:mainnet
```

#### 4.2 Devnet

```bash
yarn dev:devnet
```

#### 4.3 Custom

```bash
yarn dev --env.network=custom
```

### 5. History Mode

If you wish to remove the `/#/` from your URLs you can follow those steps https://router.vuejs.org/en/essentials/history-mode.html.

#### 5.1 Build

```bash
yarn build:mainnet --history
```

#### 5.2 Development

```bash
yarn dev --env.routerMode=history
```

## Testing

``` bash
$ yarn test
```

## Contributing

* If you find any bugs, submit an [issue](../../issues) or open a [pull-request](../../pulls), helping us catch and fix them.
* Engage with other users and developers on the [Blockpool Discord](https://discord.blockpool.io).

## Security

If you discover a security vulnerability within this package, please send an e-mail to security@ark.io. All security vulnerabilities will be promptly addressed.

## Credits

This project exists thanks to all the people who [contribute](../../contributors).

## License

[MIT](LICENSE) © [Blockpool](https://blockpool.io)
[MIT](LICENSE) © [ArkEcosystem](https://ark.io)
