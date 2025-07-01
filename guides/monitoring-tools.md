# 📊 Monitoring Your Solana Validator

Keeping your validator online and healthy is essential for rewards, reputation, and decentralization.  
Here are tools, dashboards, and tips to monitor performance like a pro.

---

## 🛠 Recommended Tools

### 🔧 Solana CLI

Use it to check block production, stake, and uptime:

```bash
solana validators
solana vote-account <your-vote-address>
solana block-production
```

---

### 🌐 Solana Beach

- Website: [https://solanabeach.io](https://solanabeach.io)
- Search for your validator to see:
  - Epoch history
  - Credits earned
  - Commission & identity

---

### 📊 Validator App

- Website: [https://validators.app](https://www.validators.app)
- Powerful analytics dashboard with filters
- Great for comparing performance across validators

---

### 📈 Stakewiz

- Website: [https://stakewiz.com](https://stakewiz.com)
- Visual uptime tracking
- Performance leaderboard
- Staking-friendly UI

---

## 🧩 Custom Tool: AndrewInUA Metrics Widget

You can embed a public-facing validator widget showing your node’s live stats.

📘 GitHub: [solana-validator-metrics-html-widget](https://github.com/AndrewInUA/solana-validator-metrics-html-widget)  
🌐 Live Preview: [andrewinua.com/#metrics](https://andrewinua.com/#metrics)

![Widget Screenshot](https://raw.githubusercontent.com/AndrewInUA/solana-validator-resources/main/assets/banner/validator-widget-preview.png)

---

## 📡 Alerts & Automation

- Use `prometheus` and `grafana` for server-side monitoring
- Set up alerting on vote skips, disk usage, or port failures
- Consider uptime bots in Discord or Telegram

---

## 🙌 Help the Ecosystem

If you’ve built a tool, dashboard, or alert system — share it here!  
We welcome contributions to this guide.

> Reliable validators are the backbone of decentralization. Monitor early, monitor often.
