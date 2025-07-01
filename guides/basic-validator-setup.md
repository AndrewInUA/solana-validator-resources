# 🛠️ Basic Validator Setup Guide (Solana)

Thinking about running your own Solana validator?  
Here’s a simplified overview of what it takes to get started — from hardware to the first block.

> 💡 This guide is meant for educational purposes. For production use, always refer to the official Solana docs.

---

## 🧰 What You Need

### ✅ Hardware (Minimum Recommended)
- CPU: 12–16 cores (e.g., AMD Ryzen 9 or Intel Xeon)
- RAM: 128GB ECC
- SSD: 1–2 TB NVMe (high endurance)
- Network: Stable 1 Gbps up/down

🛑 Do not run validators on weak VPS or cloud-only setups.

---

## 🖥️ Software Requirements

- OS: Ubuntu 22.04 LTS
- Solana CLI
- Systemd or tmux for background services

```bash
sh -c "$(curl -sSfL https://release.solana.com/stable/install)"
```

---

## 🔁 Sync the Ledger

Download snapshots to sync faster:

```bash
solana-validator \
  --identity /path/to/validator-keypair.json \
  --vote-account /path/to/vote-account-keypair.json \
  --entrypoint entrypoint.mainnet-beta.solana.com:8001 \
  --ledger /your/ledger/location \
  --expected-genesis-hash <hash> \
  --rpc-port 8899
```

📘 Use trusted sources for genesis hash and snapshot links.

---

## 🗳️ Register Your Vote Account

You need a separate vote account:

```bash
solana create-vote-account \
  vote-keypair.json \
  identity-keypair.json
```

Then link your validator to it.

---

## 🧩 Community Resources

- [Solana Validator Docs](https://docs.solana.com/running-validator/validator-reqs)
- [Discord Validator Channel](https://discord.gg/solana)

---

## ✅ Want to Learn by Example?

Check how [AndrewInUA](https://andrewinua.com) maintains high uptime, transparency, and custom tools like [this widget](https://github.com/AndrewInUA/solana-validator-metrics-html-widget).

---

> Support decentralization — or become part of it.
