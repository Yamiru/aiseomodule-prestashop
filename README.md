<p align="center">
  <img src="logo.png" alt="AiSeoModule" width="80">
</p>

<h1 align="center">AiSeoModule 2.0</h1>

<p align="center">
  <strong>Your PrestaShop store, but AI can actually find it.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PrestaShop-8.2%20|%209.x-5F259F?style=flat-square&logo=prestashop&logoColor=white" alt="PrestaShop">
  <img src="https://img.shields.io/badge/PHP-8.1+-777BB4?style=flat-square&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/Version-2.0.0-06B6D4?style=flat-square" alt="Version">
  <img src="https://img.shields.io/badge/License-Commercial-F59E0B?style=flat-square" alt="License">
  <img src="https://img.shields.io/badge/DB%20Tables-Zero-10B981?style=flat-square" alt="Zero DB">
  <img src="https://img.shields.io/badge/Files-40+-8B5CF6?style=flat-square" alt="Files">
  <img src="https://img.shields.io/badge/Languages-24-EF4444?style=flat-square" alt="Languages">
</p>

---

## 📋 Requirements

| What | Minimum |
|------|---------|
| PrestaShop | 8.2+ or 9.x |
| PHP | 8.1+ |
| cURL | enabled |
| Write access | shop root folder |

No extra libraries, no composer, no node.js.

---

## 🤔 The problem

People ask ChatGPT, search with Perplexity, talk to Alexa. Your store has meta tags and a sitemap — that worked in 2020. In 2026, AI needs structured files it can read: summaries, facts, FAQs, pricing data, knowledge graphs, tool definitions.

Most shops have none of that. This module creates all of it. Automatically.

---

## 💡 How it works

```
Your products, categories, brands, prices
            ↓
      AiSeoModule
            ↓
   40+ AI-ready files on disk
```

Install → fill in store info → click Generate → done. No database tables, no page load queries, no performance hit.

---

## 📦 What gets generated

### Search engines
`sitemap.xml` · `robots.txt` (20+ AI bots) · JSON-LD · OpenGraph · Twitter Cards · hreflang

### AI models
`llms.txt` · `llms-full.txt` · `ai/summary.json` · `ai/facts.json` · `ai/faq.json` · `ai/pricing.json` · `ai/knowledge-graph.json` · `ai.txt` · `humans.txt`

### Agentic web (March 2026)
`.well-known/webmcp.json` — Chrome 146 AI agent tools
`.well-known/agent.json` — W3C Agent Protocol discovery
`ai/commerce.json` — Google UCP for AI shopping agents
`ai/agent-manifest.json` — autonomous crawler capabilities

### Compliance & monetization
`.well-known/comp.json` — IAB CoMP v1.0 (content monetization)
`.well-known/schemamap.json` — NLWeb Schema Aggregation
`ai/compliance.json` · `ai/audit.json` · `security.txt`

Plus `ai/negotiate.json` · `ai/feed.json` · `ai/changes.xml` · `ai/datasets.json` · `ai/consensus-matrix.json` · `ai/semantic-toc.json` · `ai/contact.json` · `model-training-policy.json` and more.

---

## ⚡ After setup

| You do this | Module does this |
|-------------|-----------------|
| Add/edit a product | Pings IndexNow (6 endpoints) + sitemap ping |
| Add/edit a category | Same |
| Nothing (daily cron) | Regenerates 40+ files + Mega Ping to 24 services |
| Page loads normally | JSON-LD, OpenGraph, meta tags injected |

---

## 🔔 Mega Ping — 24 services

- **IndexNow** — 6 endpoints (Microsoft, Yandex, Seznam, Naver, Yep)
- **Sitemap Ping** — 5 search engines
- **WebSub** — 2 hubs
- **XML-RPC** — 3 services
- **AI Discovery** — 8 endpoints

---

## 🤖 AI Content Generator

Reads your actual database and writes real content:

- ✅ Store description from your categories & brands
- ✅ Keywords from top categories + newest products
- ✅ FAQ entries with real product counts, prices, descriptions
- ✅ Brand FAQs with actual price ranges
- ✅ Freshness dates set automatically
- ✅ Store info from PrestaShop config

No placeholder text. Real data from your real store.

---

## ⏰ Cron

```bash
# Once a day is enough
0 3 * * * curl -s "https://yourshop.com/module/aiseomodule/cron?token=TOKEN" > /dev/null 2>&1
```

Large shop? Split into steps. 10k+ products? Chunked mode. The module shows exact commands.

You don't need cron for everyday changes — the module pings instantly.

---

## 🛡️ Bot control

| Bot | What | Default |
|-----|------|---------|
| Googlebot | Google Search | ✅ |
| GPTBot | OpenAI training | ✅ |
| OAI-SearchBot | ChatGPT Search | ✅ |
| ChatGPT-User | ChatGPT browsing | ✅ |
| ClaudeBot | Claude AI | ✅ |
| PerplexityBot | Perplexity search | ✅ |
| Applebot | Siri & Safari | ✅ |
| Google-Extended | Gemini training | ✅ |
| CCBot | Common Crawl | ❌ |
| Bytespider | ByteDance | ❌ |

Plus 12 more toggleable bots.

---

## 🧠 Meta tags injected per page

`ai-memory-anchor` · `ai-content-density` · `ai-content-structure` · `ai-corroboration` · `ai-reading-level` · `ai-decay` · `content-valid-until` · `ai-attribution-required` · `tdm-reservation` · plus `<link>` tags for WebMCP, Schema Aggregation, CoMP, Commerce Protocol, Agent Protocol.

---

## 🌍 24 languages

🇸🇰 Slovak · 🇨🇿 Czech · 🇩🇪 German · 🇫🇷 French · 🇪🇸 Spanish · 🇮🇹 Italian · 🇵🇹 Portuguese · 🇧🇷 Brazilian Portuguese · 🇵🇱 Polish · 🇭🇺 Hungarian · 🇷🇴 Romanian · 🇳🇱 Dutch · 🇸🇪 Swedish · 🇩🇰 Danish · 🇫🇮 Finnish · 🇳🇴 Norwegian · 🇬🇷 Greek · 🇹🇷 Turkish · 🇺🇦 Ukrainian · 🇷🇺 Russian · 🇨🇳 Chinese · 🇯🇵 Japanese · 🇰🇷 Korean · 🇮🇳 Hindi

---

## 🚀 Quick install

1. Upload ZIP → install in Back Office
2. Fill in store name, org, social links
3. Click **Generate All Files**
4. Click **AI Content Generator**
5. Add one cron job
6. Copy server rules from built-in helper

---

## 📡 Protocols supported

IndexNow · WebSub · XML-RPC Ping · Sitemap Ping · llms.txt · WebMCP · IAB CoMP v1.0 · NLWeb Schema Aggregation · W3C AI Agent Protocol · Google UCP · Schema.org JSON-LD

---

## 👤 Author

**Yamiru** (Viktor Vasko)

[![Website](https://img.shields.io/badge/yamiru.com-0F172A?style=flat-square&logo=google-chrome&logoColor=white)](https://yamiru.com)
[![GitHub](https://img.shields.io/badge/GitHub-Yamiru-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Yamiru)
[![Discord](https://img.shields.io/badge/Discord-Community-5865F2?style=flat-square&logo=discord&logoColor=white)](https://discord.gg/aWSQavfPGb)

---

## 📄 License

Yamiru Commercial License — see [LICENSE](LICENSE) file.

---

<p align="center">
  <sub> Made for PrestaShop · Ready for AI · March 2026</sub>
</p>
