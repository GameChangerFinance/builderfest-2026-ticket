# 🏛️ Mainnet buy intent in GCScript DSL

This was the **original mainnet intent** used for the actual BuilderFest 2026 registration flow.

It is kept in this repository as a **historical reference** and comparison point.

## Status

- ✅ useful for studying the original real-world mainnet parameters
- 📚 useful for comparing older and newer iterations of the flow
- ⚠️ **not** the recommended starting point for new developers in this repository

For the current reference implementation and the frontend-aligned flow, use the **preprod** version instead:

- [`../preprod/README.md`](../preprod/README.md)
- [`../preprod/buy.gcscript.json`](../preprod/buy.gcscript.json)

## Why keep this file?

Because it helps developers understand how the use case evolved:

- from a live event registration intent,
- into a cleaner reference implementation,
- and toward a broader intent-based dApp architecture with reusable URLs, QRs, self-sovereign deployments, and on-chain library reuse.

## Mainnet-specific fragment

Unlike the preprod demo flow, this intent explicitly requires mainnet:

```json
{
  "require": {
    "networkTag": "mainnet"
  }
}
```

It also preserves the original event-oriented arguments, treasury, beacon, issuer, and ticket policy configuration:

```json
{
  "args": {
    "ISSUER_BEACON_POLICY": "e1ddde8138579e255482791d9fba0778cb1f5c7b435be7b3e42069de",
    "TREASURY": "addr1qx0decp93g2kwym5cz0p68thamd2t9pehlxqe02qae5r6nycv42qmjppm2rr8fj6qlzfhm6ljkd5f0tjlgudtmt5kzyqmy8x82",
    "TICKET_POLICY": "1d9c0b541adc300c19ddc6b9fb63c0bfe32b1508305ba65b8762dc7b"
  }
}
```

And, just like the newer version, it still follows the same core wallet-driven structure:

```json
{
  "run": {
    "myAddress": {
      "type": "getCurrentAddress"
    },
    "build": {
      "type": "buildTx"
    },
    "sign": {
      "type": "signTxs"
    },
    "submit": {
      "type": "submitTxs"
    }
  }
}
```

## Recommendation for new developers 💡

Use this file to understand the history, but build from the **preprod** path if your goal is to:

- run the demo quickly,
- understand the current frontend,
- learn the reusable URL/QR pattern,
- experiment with validator re-parameterization, or
- evolve the intent into a reusable on-chain library through GCFS.

## Learn more 📚

- [GameChanger Wallet repository / docs hub](https://github.com/GameChangerFinance/gamechanger.wallet)
- [GameChanger website](https://gamechanger.finance)
- [Repository root README](../../README.md)
