# 🎟️ BuilderFest 2026 Ticket Sale in GCScript DSL

> An intent-based dApp reference implementation built with **GCScript DSL** and a lightweight **HTML/JS frontend**.

👉 **Live demo:** https://builder-fest-ticket-demo.netlify.app/

This repository is meant to become a friendly, practical reference for developers who want to understand how to build **intent-based Cardano dApps** with **GameChanger Wallet** tooling and the **Universal Dapp Connector** approach.

The frontend was originally generated with the [GameChanger Wallet Playground / in-wallet code editor](https://wallet.gamechanger.finance/) and then iterated into a more guided developer experience. The result is a demo that not only lets users buy tickets, but also helps developers understand how to:

- 🧠 model a dApp as **reusable intents** rather than a tightly-coupled frontend flow
- 🧾 run the **preprod testnet** demo out of the box
- 🔁 reuse a **user-agnostic buy intent** through a sharable **URL or QR code**
- 🏗️ support **self-sovereign deployments** by re-parameterizing the validator on the user's own device
- 🌐 publish the full raw buy intent as an **on-chain reusable GCScript DSL library** via **GCFS** (GameChanger File System), so later integrations can stay tiny and QR-friendly

## ✨ Why this repo matters

This project is a nice “Rosetta Stone” example for Cardano developers:

- you can compare the same Cardano use case across DSL flavors since the original codebase was created with **TX3 DSL:** [https://github.com/txpipe/buidler-fest-2026-buy-ticket/tree/main](https://github.com/txpipe/buidler-fest-2026-buy-ticket/tree/main)
- It shows how a real-world ticketing flow can be expressed in **GCScript DSL**.
- It demonstrates how **frontend UX** and **wallet-executed intents** can collaborate cleanly.
- It highlights a very powerful pattern: once an intent is parameterized correctly, the **URL and QR become reusable distribution artifacts**.
- For Cypherpunks only: It introduces a path toward removing the frontend from the critical path entirely. Users can eventually scan a QR and execute the purchase **without any middleman web app in between!**.


## 🚦 Preprod first, ready to explore

The demo frontend is prepared to run on **Cardano preprod** out of the box.

This repository intentionally focuses on the **preprod** path as the best developer onboarding experience. The demo validator deployment used for this experience is intentionally limited in stock — **fewer than 100 tickets** are expected in this demo setup — which keeps the scenario concrete and easy to reason about.

For the up-to-date intent used by the frontend, start here:

- [`src/preprod/README.md`](./src/preprod/README.md)
- [`src/preprod/buy.gcscript.json`](./src/preprod/buy.gcscript.json)

The historical mainnet version is still included for comparison:

- [`src/mainnet/README.md`](./src/mainnet/README.md)
- [`src/mainnet/buy.gcscript.json`](./src/mainnet/buy.gcscript.json)

## 🗂️ Repository structure

```text
.
├── README.md
├── LICENSE
├── serve.sh
├── src/
│   ├── mainnet/
│   │   ├── README.md
│   │   └── buy.gcscript.json
│   └── preprod/
│       ├── README.md
│       ├── buy.QR.png
│       ├── buy.URL.txt
│       └── buy.gcscript.json
└── www/
    └── index.html
```

## 🚀 Quick start

### 1) Install the only required local dependency

This repository serves the frontend with Python's built-in HTTP server:

```bash
python3 --version
```

If Python 3 is missing:

- **Ubuntu / Debian**
  ```bash
  sudo apt update
  sudo apt install python3
  ```
- **macOS**: Python 3 is often already available, otherwise install it with your preferred package manager.
- **Windows**: install Python 3 and make sure it is available in your terminal.

### 2) Run the local server

Make the script executable once if needed:

```bash
chmod +x ./serve.sh
```

Then run:

```bash
./serve.sh
```

This serves the `www/` folder locally using:

```bash
python3 -m http.server -d www
```

Now open the local address printed by Python in your browser.

## 📲 Reusable buy intent: URL + QR

One of the nicest things about intent-based dApps is that the final interaction artifact can often be shared directly.

In this repository, the preprod buy flow already has:

- a reusable URL: [`src/preprod/buy.URL.txt`](./src/preprod/buy.URL.txt)
- a reusable QR code: [`src/preprod/buy.QR.png`](./src/preprod/buy.QR.png)

You can also open the buy intent directly in GameChanger Wallet here:

[👉 Open the reusable preprod buy intent](https://wallet.gamechanger.finance/api/2/run/1-H4sIAAAAAAAAA21U247bNhD9FUIvaYG98CqKfmrSIm2BogiyLfpQFMGIHNqydTNJ2ZYW---l7M0GKCpBgnjOYObMkEfPRZpHLDZFtKEZU3FXpCa1K_BhmgmQ1NgDrrDDW0Qz9Jn8NAW7g4hvESQNZISQF80ICUnTk7RDgifs0wP5awiHSOqZNN045KB-e2WbPmWaxCFnQ2IHh8SHoSPQk6G_zwVyloBThLpF0jZ1gDCTmIaAjpwaID__-PGJ-KbFOMeEHRnDkAY7tFkuXtZC72PW-sdV4E-QIOMQthl7fm33voV-m0PGdkpT_HISOeKVyd3tMuO0Z8yImkupWOUtKgsKmNU1t1JIKkVlq7yW4Cpd0wo0RcQavyWKzZLHyUtD3yBwLmBcta1fXxLGxJaQ2uXiu1ksQrSVQe9Gq_G0dce5CjMPwrio7VZN1Rlo33WH0pnkFmkX048i7EeAwA_BpiXy0PKUepz5oT3w_fF83Ed3-iZpSpfha4NcWF8ylbPXslKylBZphV5K47jQmlLHLUVWljUHVnNda-k8FUwYBt5a_p-sTe_wUmzYXVEj2LyL49A2dv7V5VIMkDpkymhelQax1BoYpyBdSbXwhlWu8iU6xZQHlGi1rhmCKd6SQYyYfocOf1mLFEooKVl-lPKSSyVZ3hIvUXldZoVcUFHmdymMqMSqNAWEOIX5f3fgGFqqJxOjS-6cll1IdAkhaDPj_rLzpy52-2T2l-MMCz2ksZzd1B53qQxmka2j-y4KEFZvz1JNgp92lvvkRu7LcDwtlO_PV3eth_HeDjEVG0Wv18tdETBNoV8PZpddkGW1kANWYrqiN9-ge7q5NCOvtr0R7-PTV_veDnjxvMX03bt18e77lwyvvio2fxdb6-Pm8bFWJTV52s4aRm1pKqY41RzrGspaodLc2UpRU3lZcTDOOAVaAj58mJrWYfiYB_ZDC-vccrYY7GM9zQ9b-_oX-eflrac_P__2CVLCtbtil9KY4-nD9d5UufnH4uVfWRdRFIQEAAA?networkTag=preprod)

[![🎟️ Scan to buy on preprod](./src/preprod/buy.QR.png)](https://wallet.gamechanger.finance/api/2/run/1-H4sIAAAAAAAAA21U247bNhD9FUIvaYG98CqKfmrSIm2BogiyLfpQFMGIHNqydTNJ2ZYW---l7M0GKCpBgnjOYObMkEfPRZpHLDZFtKEZU3FXpCa1K_BhmgmQ1NgDrrDDW0Qz9Jn8NAW7g4hvESQNZISQF80ICUnTk7RDgifs0wP5awiHSOqZNN045KB-e2WbPmWaxCFnQ2IHh8SHoSPQk6G_zwVyloBThLpF0jZ1gDCTmIaAjpwaID__-PGJ-KbFOMeEHRnDkAY7tFkuXtZC72PW-sdV4E-QIOMQthl7fm33voV-m0PGdkpT_HISOeKVyd3tMuO0Z8yImkupWOUtKgsKmNU1t1JIKkVlq7yW4Cpd0wo0RcQavyWKzZLHyUtD3yBwLmBcta1fXxLGxJaQ2uXiu1ksQrSVQe9Gq_G0dce5CjMPwrio7VZN1Rlo33WH0pnkFmkX048i7EeAwA_BpiXy0PKUepz5oT3w_fF83Ed3-iZpSpfha4NcWF8ylbPXslKylBZphV5K47jQmlLHLUVWljUHVnNda-k8FUwYBt5a_p-sTe_wUmzYXVEj2LyL49A2dv7V5VIMkDpkymhelQax1BoYpyBdSbXwhlWu8iU6xZQHlGi1rhmCKd6SQYyYfocOf1mLFEooKVl-lPKSSyVZ3hIvUXldZoVcUFHmdymMqMSqNAWEOIX5f3fgGFqqJxOjS-6cll1IdAkhaDPj_rLzpy52-2T2l-MMCz2ksZzd1B53qQxmka2j-y4KEFZvz1JNgp92lvvkRu7LcDwtlO_PV3eth_HeDjEVG0Wv18tdETBNoV8PZpddkGW1kANWYrqiN9-ge7q5NCOvtr0R7-PTV_veDnjxvMX03bt18e77lwyvvio2fxdb6-Pm8bFWJTV52s4aRm1pKqY41RzrGspaodLc2UpRU3lZcTDOOAVaAj58mJrWYfiYB_ZDC-vccrYY7GM9zQ9b-_oX-eflrac_P__2CVLCtbtil9KY4-nD9d5UufnH4uVfWRdRFIQEAAA?networkTag=preprod)

Because the intent is generally **user-agnostic**, the same URL/QR can be distributed broadly. The wallet resolves the active user context at execution time.

## 🧩 GCScript at a glance

The buy flow is powered by an on-chain reusable library which contains the full intent implementation. 

Import the library, execute the intent with some custom arguments, then capture the results at frontend:

```json
{
  "type": "script",
  "title": "Buy a ticket",
  "description": "Purchase a ticket to participate in the event. Works by importing the intent source code from an on-chain reusable library stored via GCFS filesystem protocol",
  "exportAs": "TicketData",
  "args": {
    "script-lang": "plutus_v3",
    "script-hash": "d7f1193b244518fce5ca5a1c7b2c4340438c8a1c4ad87b08a70eeebe",
    "script-size": 2690,
    "script-address": "addr_test1zrtlzxfmy3z33l89efdpc7evgdqy8ry2r39ds7cg5u8wa0nmmk6d9tdz4cz9np3rjpaar2krctzs2rl2ttney2klk2jqwqjsdv",
    "script-utxo-hash": "23cf61539db485464ce08ef449d237700d2c0e166b2a1b27b74df031391afcc2",
    "script-utxo-index": 1,
    "beacon-policyId": "1ae0de15972869ee677a120a4d6073f918d8f6ed515fae4ec77b1ea9",
    "beacon-assetNameHex": "53544154455f424541434f4e5f76313230363236393832",
    "treasury-address": "addr_test1qrl07u9ssdtdwtzhrt0zrrr79yejxhfvmsmjt9jxqyaz0ktp6ydulqht6r9z4ld0jms3a3c7gw45u32vhc2ftdp2f6rqvz02jw",
    "ticket-cost": 5000000
  },
  "return": {
    "mode": "last"
  },
  "run": {
    "importedScript": {
      "type": "importAsScript",
      "args": "{get('args')}",
      "from": [
        "gcfs://b5609d8fdc910c698152072ebba6b5e572dc85098f482a9d9d5a74ae.BuilderFest@latest://src/buy.gcscript"
      ]
    }
  },
  "returnURLPattern": "http://0.0.0.0:8000/"
}
```

And the overal design of the on-chain library is mainly: 

**query last ticket state → compute the next ticket state → build the transaction with next state → ask the wallet to sign → submit**. 🎯

## 🏗️ Self-sovereign deployment and on-chain reuse

This repository also documents a bigger idea than “buying a ticket”.

The frontend is designed to help developers move toward a fully self-sovereign flow where users can:

1. re-parameterize the validator on their own device,
2. produce their own deployment artifacts,
3. publish the full raw buy intent as a **reusable on-chain GCScript DSL library** using **GCFS**, and
4. replace larger downstream integrations with smaller wrapper intents that import and reuse that published logic.

That matters because it leads to:

- ✂️ smaller final integration code
- 📦 easier QR packing
- 🔓 less dependence on a hosted frontend
- 🤝 a more open, forkable, inspectable ecosystem

## 🌱 New to GameChanger?

A good next step is to explore the official GameChanger Wallet repository and docs:

- [GameChanger Wallet repository / docs hub](https://github.com/GameChangerFinance/gamechanger.wallet)
- [GameChanger website](https://gamechanger.finance)
- [GameChanger Wallet / Playground](https://wallet.gamechanger.finance/playground)

## 💡 Suggested learning path

If this is your first time with this repo, a fun path is:

1. run the frontend using the online demo,
2. buy some tickets using the frontend and using the QR code,
3. hacker mode: inspect the buy intent using the wallet live debugger,
4. inspect the buy intent in the HTML file,
5. run the frontend locally,
6. play/modify the HTML file,
7. run the new frontend locally,
8. compare this repo with the original TX3 version,
9. then imagine how you would publish part of the logic on-chain for reuse.

Have fun and happy hacking! ✨

## Disclaimer

This was made for educational purposes to keep the example developer-friendly. Mind to add more validations for any production release!

## 📄 License

This repository is licensed under the [MIT License](./LICENSE).
