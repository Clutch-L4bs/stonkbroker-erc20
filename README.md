# $STONKBROKER ERC-20

Public source for the **$STONKBROKER** (`STONKBROKER`) fixed-supply ERC-20 on **Robinhood Chain** (chain ID `4663`).

| | |
|---|---|
| **Name** | StonkBroker |
| **Symbol** | STONKBROKER |
| **Decimals** | 18 |
| **Address** | [`0xe934e36a439c94017b64a3fece66af12099abf50`](https://robinhoodchain.blockscout.com/token/0xe934e36a439c94017b64a3fece66af12099abf50) |
| **Standard** | ERC-20 + Burnable + Permit (OpenZeppelin) |
| **Issuer** | Clutch Labs, LLC (New York, United States) |

## Contract properties

- Fixed supply minted once in the constructor
- No owner / admin after deploy
- No post-deploy mint
- No pause, freeze, blacklist, or upgrade proxy
- No transfer fees or on-contract staking
- Optional self-burn (`ERC20Burnable`)

## Docs

- Whitepaper: https://stonkbrokers.io/docs/stonkbroker-token
- Docs hub: https://stonkbrokers.io/docs
- HasLock Certified Audit: https://stonkbrokers.io/docs/HasLock-Certified-Audit-STONKBROKER-ERC20.pdf
- HasLock Penetration Assessment: https://stonkbrokers.io/docs/HasLock-Penetration-Assessment-STONKBROKER-ERC20.pdf

## Build

OpenZeppelin Contracts is a git submodule pinned at v5.0.2 (`lib/openzeppelin-contracts`).

```bash
git clone --recurse-submodules https://github.com/Clutch-L4bs/stonkbroker-erc20.git
cd stonkbroker-erc20
forge build
```

In an existing clone, run `git submodule update --init` before `forge build`.

## License

BUSL-1.1 — see `LICENSE`. Change Date **2029-08-25** → MIT.
