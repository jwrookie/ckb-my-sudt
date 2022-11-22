# my-sudt

Prerequisites

```sh
capsule --version  
Capsule 0.9.0 f43d045 or later
# repo: https://github.com/TheWaWaR/capsule

ckb-cli --version
ckb-cli 1.3.0 (2dd2269 2022-11-20) or later
# repo: https://github.com/nervosnetwork/ckb-cli
```

Run tests:

``` sh
capsule test
```

Build contracts:

``` sh
capsule build --release
```

Deploy contracts:

```sh
capsule deploy --api https://testnet.ckbapp.dev/rpc --address ckt1qyqycw7paxj6d9ajv75846j9a39fk3pl96hsujejqd

# use `capsule deploy --help` to get more details of deploy
```

- password: the password when creating the account, not the private key

- If it prompts that your cell balance is not enough, you should go to [faucet](https://faucet.nervos.org/) claim some cells

- If the fee rate is not enough, you should delete the `migrations` folder, and follow the prompts to give the correct fee rate, use --fee
