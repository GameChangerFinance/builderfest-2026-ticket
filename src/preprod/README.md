# 🧪 Preprod buy intent in GCScript DSL

This is the **current pre-production testnet** version of the ticket purchase intent, aligned with the newer frontend implementation in this repository.

If you are exploring this project for the first time, **start here**. ✅

## Why this version matters

This preprod intent is the most relevant one for developers because it is:

- 🎯 the version prepared to work with the current frontend flow
- 🧪 ready for **Cardano preprod** out of the box
- 🔁 easy to distribute as a **reusable URL or QR code**
- 🏗️ a solid base for experimenting with **self-sovereign validator deployments**
- 🌐 ready to evolve toward **on-chain intent-library reuse through GCFS**

The demo validator deployment behind this experience is intentionally limited in stock, with **fewer than 100 tickets** expected in this demo setup.

## Open the intent directly

- 👉 [Open the preprod buy intent in GameChanger Wallet](https://wallet.gamechanger.finance/api/2/run/1-H4sIAAAAAAAAA21U247bNhD9FUIvaYG98CqKfmrSIm2BogiyLfpQFMGIHNqydTNJeS0t9t9L2c4GKCpAgnhmdObMkEcvRZpHLDZFtKEZU3FXpCa1K_BhmgmQ1NgDrrDDa0Yz9Dn4aQp2BxHfMkgayAghL5oREpKmJ2mHBE_Ypwfy1xAOkdQzabpxyEn99hJt-pTDJA6ZDYkdHBIfho5AT4b-PhfILAGnCHWLpG3qAGEmMQ0BHTk1QH7-8eMT8U2LcY4JOzKGIQ12aLNcPK-F3ses9Y-LwJ8gQcYhbDP2cmv3voV-m1PGdkpT_HISOeMWyd3tcsRpz5gRNZdSscpbVBYUMKtrbqWQVIrKVnktwVW6phVoiog1fiOKzZLHyUtD3yBwLmBcta1vXxLGxJaQ2uXsu1ksQrSVQe9Gq_G0dce5CjMPwrio7VZN1TPQvusOpTPJLdIuph9F2I8AgR-CTUvkoeUp9TjzQ3vg--PzcR_d6ZukKZ2Hrw1yYX3JVGavZaVkKS3SCr2UxnGhNaWOW4qsLGsOrOa61tJ5KpgwDLy1_D-sTe_wXGzYXVEj2LyL49A2dv7V5VIMkDpkymhelQax1BoYpyBdSbXwhlWu8iU6xZQHlGi1rhmCKd7IIEZMv0OHv6xFCiWUlCzfSnnJpZIsb4mXqLwus0IuqCjzsxRGVGJVmgJCnML8vztwDC3Vk4nRJfecll1IdAkhaDPj_rzzpy52-2T25-MMCz2ksZzd1B53qQxmka2j-y4KEFZvn6WaBD_tLPfJjdyX4XhaKN8_X9y1HsZ7O8RUbBS9XK93RcA0hX49mF12QZbVQk5YA9MFvfoG3dPVpRm52fYaeB-fvtr3esCLly2m796ti3ffv2Z49VWx-bvYWh83j4-1KqnJ03bWMGpLUzHFqeZY11DWCpXmzlaKmsrLioNxxinQEvDhw9S0DsPHPLAfWljnltlisI_1ND9s7e0v8s_rW09_fv7tE6SEa3fFLqXxUv7Kcu_z9_e3kTjshoceU9v4-QHG8bF4_ReOhL_unQQAAA?networkTag=preprod)
- 📝 [Plain-text URL](./buy.URL.txt)
- 🧾 [Full source intent](./buy.gcscript.json)

[![🎟️ Scan the QR to buy on preprod](./buy.QR.png)](https://wallet.gamechanger.finance/api/2/run/1-H4sIAAAAAAAAA21U247bNhD9FUIvaYG98CqKfmrSIm2BogiyLfpQFMGIHNqydTNJeS0t9t9L2c4GKCpAgnhmdObMkEcvRZpHLDZFtKEZU3FXpCa1K_BhmgmQ1NgDrrDDa0Yz9Dn4aQp2BxHfMkgayAghL5oREpKmJ2mHBE_Ypwfy1xAOkdQzabpxyEn99hJt-pTDJA6ZDYkdHBIfho5AT4b-PhfILAGnCHWLpG3qAGEmMQ0BHTk1QH7-8eMT8U2LcY4JOzKGIQ12aLNcPK-F3ses9Y-LwJ8gQcYhbDP2cmv3voV-m1PGdkpT_HISOeMWyd3tcsRpz5gRNZdSscpbVBYUMKtrbqWQVIrKVnktwVW6phVoiog1fiOKzZLHyUtD3yBwLmBcta1vXxLGxJaQ2uXsu1ksQrSVQe9Gq_G0dce5CjMPwrio7VZN1TPQvusOpTPJLdIuph9F2I8AgR-CTUvkoeUp9TjzQ3vg--PzcR_d6ZukKZ2Hrw1yYX3JVGavZaVkKS3SCr2UxnGhNaWOW4qsLGsOrOa61tJ5KpgwDLy1_D-sTe_wXGzYXVEj2LyL49A2dv7V5VIMkDpkymhelQax1BoYpyBdSbXwhlWu8iU6xZQHlGi1rhmCKd7IIEZMv0OHv6xFCiWUlCzfSnnJpZIsb4mXqLwus0IuqCjzsxRGVGJVmgJCnML8vztwDC3Vk4nRJfecll1IdAkhaDPj_rzzpy52-2T25-MMCz2ksZzd1B53qQxmka2j-y4KEFZvn6WaBD_tLPfJjdyX4XhaKN8_X9y1HsZ7O8RUbBS9XK93RcA0hX49mF12QZbVQk5YA9MFvfoG3dPVpRm52fYaeB-fvtr3esCLly2m796ti3ffv2Z49VWx-bvYWh83j4-1KqnJ03bWMGpLUzHFqeZY11DWCpXmzlaKmsrLioNxxinQEvDhw9S0DsPHPLAfWljnltlisI_1ND9s7e0v8s_rW09_fv7tE6SEa3fFLqXxUv7Kcu_z9_e3kTjshoceU9v4-QHG8bF4_ReOhL_unQQAAA?networkTag=preprod)

## Why the URL and QR are reusable

A lovely property of intents is that they are often **user-agnostic**.

This buy intent does not hardcode the final receiver wallet of the ticket. Instead, it resolves the active wallet address when the user executes it:

```json
{
  "myAddress": {
    "type": "getCurrentAddress"
  }
}
```

That means the same URL or QR can be shared with many users. Each user runs the same intent, but the wallet injects **their own active address** at execution time. 🎉

## What the intent does

At a high level, this script:

1. queries the validator state through the beacon token,
2. computes the current and next ticket number,
3. builds a transaction that pays the treasury and mints the ticket token,
4. signs the transaction in the user's wallet,
5. submits it, and
6. exports useful result data.

Main/root code of block basically will run the intent workflow on user-devices (desktop and mobile, yes) and will craft in the end suitable exports for the frontend to aggregate the results:

```json5
{
  "type": "script",
  "title": "Buy a ticket",
  "description": "Purchase a ticket to participate in the event",
  "exportAs": "TicketData", // name of the export
  "return": {
    "mode": "last" // will return back to frontend the results of the function call named arbitrarely "finally" 
  },
  "returnURLPattern": "http://0.0.0.0:8000/", // where to send back the exported results (like a handy webhook!)
  "run"{
    //...workflow here ...
    "finally": {
        "type": "macro",
        "run": {
            "{join('.',get('cache.ticketToken.policyId'),get('cache.ticketToken.assetName'))}": {
                "txHash": "{get('cache.build.txHash')}",
                "address": "{get('cache.myAddress')}",
                "ticketNumber": "{get('cache.ticketNumber.current')}",
                "ticketToken": "{get('cache.ticketToken')}",
                "ticketCost": "{get('args.ticket-cost')}",
                "ttl": {
                    "from": "{get('cache.currentSlotNumber')}",
                    "to": "{addBigNum(get('cache.currentSlotNumber'),'600')}"
                },
                "newState": {
                    "ticketNumber": "{get('cache.ticketNumber.next')}",
                    "utxo": {
                        "txHash": "{get('cache.build.txHash')}",
                        "index": "{get('cache.build.indexMap.output.outputWithTheAdminTokenAndDatum')}"
                    }
                }
            }
        }
    }
  }
}

```

The query phase looks like this:

```json
{
  "beacon": {
    "type": "query",
    "get": {
      "kind": "BeaconToken",
      "asset": {
        "policyId": "{get('args.beacon-policyId')}",
        "assetNameHex": "{get('args.beacon-assetNameHex')}"
      },
      "address": "{get('args.script-address')}"
    }
  }
}
```

And the transaction assembly stage is where the actual ticket purchase is expressed:

```json
{
    "build": {
        "type": "buildTx",
        "title": "{replaceAll( '🚀 BuilderFest 2026 Ticket #%', '%', get('cache.ticketNumber.current') )}",
        "tx": {
            "inputs": [
                {
                    "txHash": "{get('cache.beacon.txHash')}",
                    "index": "{get('cache.beacon.index')}"
                }
            ],
            "mints": [
                {
                    "policyId": "{get('cache.ticketToken.policyId')}",
                    "assets": [
                        {
                            "assetName": "{get('cache.ticketToken.assetName')}",
                            "quantity": "1"
                        }
                    ]
                }
            ],
            "outputs": {
                "withPayment": {
                    "address": "{get('args.treasury-address')}",
                    "assets": [
                        {
                            "policyId": "ada",
                            "assetName": "ada",
                            "quantity": "{addBigNum(get('args.ticket-cost'),0)}"
                        }
                    ]
                },
                "withTicket": {
                    "address": "{get('cache.myAddress')}",
                    "assets": [
                        {
                            "policyId": "{get('cache.ticketToken.policyId')}",
                            "assetName": "{get('cache.ticketToken.assetName')}",
                            "quantity": "1"
                        }
                    ]
                },
                "withAdminTokenAndNextState": {
                    "address": "{get('args.script-address')}",
                    "assets": [
                        {
                            "policyId": "{get('args.beacon-policyId')}",
                            "assetNameHex": "{get('args.beacon-assetNameHex')}",
                            "quantity": "1"
                        }
                    ],
                    "datum": {
                        "datumHex": "{get('cache.nextState.dataHex')}"
                    },
                    "idPattern": "outputWithTheAdminTokenAndDatum"
                }
            },
            "witnesses": {
                "plutus": {
                    "scripts": [
                        {
                            "scriptHashHex": "{get('args.script-hash')}",
                            "lang": "{get('args.script-lang')}",
                            "scriptSize": "{get('args.script-size')}",
                            "input": {
                                "txHash": "{get('args.script-utxo-hash')}",
                                "index": "{get('args.script-utxo-index')}"
                            }
                        }
                    ]
                }
            },
            "ttl": {
                "from": "{get('cache.currentSlotNumber')}",
                "until": "{addBigNum(get('cache.currentSlotNumber'),'600')}"
            },
            "auxiliaryData": {
                "674": {
                    "msg": [
                        "🚀 Cardano BuilderFest 2026 Registration:\n",
                        "{replaceAll( '- Ticket: %', '%', get('cache.ticketNumber.current') )}",
                        "\n",
                        "{replaceAll( '- Cost: % lovelaces', '%', get('args.ticket-cost') )}",
                        "\n\n",
                        "✨ Created with GCScript DSL:\n",
                        "- https://github.com/GameChangerFinance",
                        "/builderfest-2026-ticket\n",
                        "\n",
                        "- Website: https://gamechanger.finance\n",
                        "\n"
                    ]
                }
            },
            "options": {
                "collateralCoinSelection": "LASLAD"
            }
        }
    }
}
```

## Self-sovereign deployments 🚀

This full source code can be split and evolved into a **self-sovereign deployment flow** from the frontend itself.

The big idea is:

- the user re-parameterizes the Plutus validator locally,
- deployment artifacts are produced on the user's own device,
- the full raw buy intent can then be published as a reusable artifact,
- and future integrations can become much smaller wrappers.

That is a very empowering pattern for open Cardano apps: users and teams can deploy, inspect, remix, and redistribute flows without depending on a single hosted frontend.

## GCFS + on-chain intent-library reuse 🌐

Another important concept in this repository is that the full buy intent can be transformed into an **on-chain reusable library** using **GCFS**, the GameChanger on-chain filesystem protocol.

Why bother?

Because once the larger raw logic is stored on-chain and reused from there, the final buy integration can become much smaller:

- ✂️ less code in the final integration
- 📦 more QR-friendly payloads
- 🔁 easier distribution
- 🚫 no middleman frontend required for the final user flow

That is exactly what makes the QR approach especially exciting here: users can scan and buy their own tickets directly with wallet-driven execution.

## Suggested local dev flow

From the repository root:

```bash
chmod +x ./serve.sh
./serve.sh
```

This serves the `www/` frontend locally with Python 3. If you do not have Python installed yet, install `python3` first and re-run the command.

## Learn more 📚

To go deeper into the GameChanger ecosystem:

- [GameChanger Wallet repository / docs hub](https://github.com/GameChangerFinance/gamechanger.wallet)
- [GameChanger website](https://gamechanger.finance)
- [Open GameChanger Wallet](https://wallet.gamechanger.finance)

Happy hacking, and enjoy exploring intent-based Cardano UX ✨
