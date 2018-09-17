# BPL Explorer 3.0

<p align="center">
    <img src="/banner.png" />
</p>

> Designed and developed from the ground-up, using lean & fast developmental frameworks (Tailwind CSS & Vue.JS).

[![Build Status](https://badgen.now.sh/travis/blockpool-io/explorer-3.0/master)](https://travis-ci.org/blockpool-io/explorer-3.0)
[![License: MIT](https://badgen.now.sh/badge/license/MIT/green)](https://opensource.org/licenses/MIT)

You can access it at [https://explorer.blockpool.io/](https://explorer.blockpool.io/)

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

#### 3.2 Testnet

```bash
yarn build:testnet
```

#### 3.3 Custom

```bash
yarn build --network my-custom-network
```

#### 3.4 GitHub Pages

If you are going to host your explorer instance on GitHub Pages you will need to specify your base url in most cases as GitHub Pages serves repositories from sub-directories instead of sub-domains.

```bash
yarn build --base https://username.github.io/repository/
```

#### 3.5 Run Express Server

You can run the explorer as an express server. This makes it a little more light-weight but not needing to have services such as apache or nginx.

```bash
EXPLORER_HOST="127.0.0.1" EXPLORER_PORT="4200" node express-server.js
```

### 4. Development

#### 4.1 Mainnet

```bash
yarn dev # or yarn dev:mainnet
```

#### 4.2 Testnet

```bash
yarn dev:testnet
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

> Keep in mind that this requires you to run your own server and a running instance of nginx.

## Testing

``` bash
$ yarn test
```

## Security

If you discover a security vulnerability within this package, please send an e-mail to support@blockpool.io. All security vulnerabilities will be promptly addressed.

## Contributing

* If you find any bugs, submit an [issue](../../issues) or open a [pull-request](../../pulls), helping us catch and fix them.
* Engage with other users and developers on [Discord](https://discord.blockpool.io/).

## Credits

- [Brian Faust](https://github.com/faustbrian)
- [Lúcio Rubens](https://github.com/luciorubeens)
- [Alex Barnsley](https://github.com/alexbarnsley)
- [Edgar Goetzendorff](https://github.com/dated)
- [All Contributors](../../contributors)

## License

[MIT](LICENSE) © [Blockpool](https://blockpool.io)
