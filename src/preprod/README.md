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

- 👉 [Open the preprod buy intent in GameChanger Wallet](https://wallet.gamechanger.finance/api/2/run/1-H4sIAAAAAAAAA21U247bNhD9FUIvaYG98CqKfmrSIm2BogiyLfpQFMGIHNqydTNJ2ZYW---l7M0GKCpBgnjOYObMkEfPRZpHLDZFtKEZU3FXpCa1K_BhmgmQ1NgDrrDDW0Qz9Jn8NAW7g4hvESQNZISQF80ICUnTk7RDgifs0wP5awiHSOqZNN045KB-e2WbPmWaxCFnQ2IHh8SHoSPQk6G_zwVyloBThLpF0jZ1gDCTmIaAjpwaID__-PGJ-KbFOMeEHRnDkAY7tFkuXtZC72PW-sdV4E-QIOMQthl7fm33voV-m0PGdkpT_HISOeKVyd3tMuO0Z8yImkupWOUtKgsKmNU1t1JIKkVlq7yW4Cpd0wo0RcQavyWKzZLHyUtD3yBwLmBcta1fXxLGxJaQ2uXiu1ksQrSVQe9Gq_G0dce5CjMPwrio7VZN1Rlo33WH0pnkFmkX048i7EeAwA_BpiXy0PKUepz5oT3w_fF83Ed3-iZpSpfha4NcWF8ylbPXslKylBZphV5K47jQmlLHLUVWljUHVnNda-k8FUwYBt5a_p-sTe_wUmzYXVEj2LyL49A2dv7V5VIMkDpkymhelQax1BoYpyBdSbXwhlWu8iU6xZQHlGi1rhmCKd6SQYyYfocOf1mLFEooKVl-lPKSSyVZ3hIvUXldZoVcUFHmdymMqMSqNAWEOIX5f3fgGFqqJxOjS-6cll1IdAkhaDPj_rLzpy52-2T2l-MMCz2ksZzd1B53qQxmka2j-y4KEFZvz1JNgp92lvvkRu7LcDwtlO_PV3eth_HeDjEVG0Wv18tdETBNoV8PZpddkGW1kANWYrqiN9-ge7q5NCOvtr0R7-PTV_veDnjxvMX03bt18e77lwyvvio2fxdb6-Pm8bFWJTV52s4aRm1pKqY41RzrGspaodLc2UpRU3lZcTDOOAVaAj58mJrWYfiYB_ZDC-vccrYY7GM9zQ9b-_oX-eflrac_P__2CVLCtbtil9KY4-nD9d5UufnH4uVfWRdRFIQEAAA?networkTag=preprod)
- 📝 [Plain-text URL](./buy.URL.txt)
- 🧾 [Full source intent](./buy.gcscript.json)

[![🎟️ Scan the QR to buy on preprod](./buy.QR.png)](https://wallet.gamechanger.finance/api/2/run/1-H4sIAAAAAAAAA21U247bNhD9FUIvaYG98CqKfmrSIm2BogiyLfpQFMGIHNqydTNJ2ZYW---l7M0GKCpBgnjOYObMkEfPRZpHLDZFtKEZU3FXpCa1K_BhmgmQ1NgDrrDDW0Qz9Jn8NAW7g4hvESQNZISQF80ICUnTk7RDgifs0wP5awiHSOqZNN045KB-e2WbPmWaxCFnQ2IHh8SHoSPQk6G_zwVyloBThLpF0jZ1gDCTmIaAjpwaID__-PGJ-KbFOMeEHRnDkAY7tFkuXtZC72PW-sdV4E-QIOMQthl7fm33voV-m0PGdkpT_HISOeKVyd3tMuO0Z8yImkupWOUtKgsKmNU1t1JIKkVlq7yW4Cpd0wo0RcQavyWKzZLHyUtD3yBwLmBcta1fXxLGxJaQ2uXiu1ksQrSVQe9Gq_G0dce5CjMPwrio7VZN1Rlo33WH0pnkFmkX048i7EeAwA_BpiXy0PKUepz5oT3w_fF83Ed3-iZpSpfha4NcWF8ylbPXslKylBZphV5K47jQmlLHLUVWljUHVnNda-k8FUwYBt5a_p-sTe_wUmzYXVEj2LyL49A2dv7V5VIMkDpkymhelQax1BoYpyBdSbXwhlWu8iU6xZQHlGi1rhmCKd6SQYyYfocOf1mLFEooKVl-lPKSSyVZ3hIvUXldZoVcUFHmdymMqMSqNAWEOIX5f3fgGFqqJxOjS-6cll1IdAkhaDPj_rLzpy52-2T2l-MMCz2ksZzd1B53qQxmka2j-y4KEFZvz1JNgp92lvvkRu7LcDwtlO_PV3eth_HeDjEVG0Wv18tdETBNoV8PZpddkGW1kANWYrqiN9-ge7q5NCOvtr0R7-PTV_veDnjxvMX03bt18e77lwyvvio2fxdb6-Pm8bFWJTV52s4aRm1pKqY41RzrGspaodLc2UpRU3lZcTDOOAVaAj58mJrWYfiYB_ZDC-vccrYY7GM9zQ9b-_oX-eflrac_P__2CVLCtbtil9KY4-nD9d5UufnH4uVfWRdRFIQEAAA?networkTag=preprod)

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
