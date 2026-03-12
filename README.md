
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
  <img src="https://img.shields.io/badge/Files%20Generated-27+-8B5CF6?style=flat-square" alt="Files">
</p>

---

## 📋 Requirements

Before you install, make sure you have:

| What | Minimum |
|------|---------|
| PrestaShop | 8.2+ or 9.x |
| PHP | 8.1 or newer |
| cURL | enabled (for pinging search engines) |
| Write access | on your shop root folder (the module saves files there) |

That's it. No extra libraries, no composer, no node.js.

---

## 🤔 What's the problem?

People don't just use Google anymore. They ask **ChatGPT**, search with **Perplexity**, use **Claude**, talk to **Alexa**. And when they do — your store is invisible. AI doesn't know it exists.

Regular SEO (meta tags, sitemaps) still matters, but it's not enough. AI models need **structured files** they can read — summaries, facts, FAQs, pricing data, knowledge graphs.

Most e-shops don't have any of that. This module creates all of it automatically.

---

## 💡 What does it do?

You install it, click one button, and the module reads your PrestaShop database — your products, categories, brands, prices — and creates **27+ files** that AI systems understand.

```
Your store data  →  AiSeoModule  →  27+ AI-readable files on disk
```

No database tables created. No queries on page load. Just static files your web server handles. **Zero performance impact.**

---

## 📦 What gets created?

### For search engines
- `sitemap.xml` — split sitemaps with image support
- `robots.txt` — rules for 20+ AI bots
- JSON-LD schemas — Product, Organization, FAQ, Breadcrumb
- OpenGraph & Twitter Cards

### For AI models
- `llms.txt` — plain-text store overview (what LLMs read first)
- `llms-full.txt` — full Markdown with 200 products (for RAG)
- `ai/summary.json` — machine-readable store summary
- `ai/facts.json` — clean key-value facts
- `ai/faq.json` — auto-generated FAQ (up to 100 entries)
- `ai/pricing.json` — product catalog with prices & EANs
- `ai/knowledge-graph.json` — entity data
- `ai/agent-manifest.json` — for autonomous AI shoppers

### For trust & compliance
- `humans.txt` — E-E-A-T author info
- `security.txt` — RFC 9116 security contact
- `.well-known/ai-policy.json` — AI usage policy
- `.well-known/ai-license.json` — content licensing
- GDPR & EU AI Act compliance signals

---

## 🚀 Setup (5 minutes)

```
Step 1  →  Upload ZIP & install the module
Step 2  →  Fill in store name, organization, social links
Step 3  →  Click "Generate All Files"
Step 4  →  Click "AI Content Generator" (reads your DB, writes real content)
Step 5  →  Add one cron job for daily refresh
Step 6  →  Copy .htaccess / nginx rules from the built-in helper
```

**Done.** Everything else is automatic.

---

## ⚡ What happens after setup?

You don't have to do anything. The module works in the background:

| You do this | Module does this |
|------------|-----------------|
| Add/edit a product | Pings IndexNow (6 endpoints) + sitemap ping |
| Add/edit a category | Same thing |
| Nothing (daily cron) | Regenerates all 27+ files + Mega Ping to 24 services |
| Page loads normally | JSON-LD, OpenGraph, meta tags injected automatically |

---

## 🔔 Mega Ping (24 services)

When something changes, the module doesn't just wait for Google to notice. It actively notifies:

- **IndexNow** — 6 endpoints (Microsoft, Yandex, Seznam, Naver, Yep)
- **Sitemap Ping** — 5 search engines
- **WebSub** — 2 hubs (Google, Superfeedr)
- **XML-RPC** — 3 services
- **AI Discovery** — 8 file endpoints

---

## ⏰ Cron

One line, once a day, that's all:

```bash
0 3 * * * curl -s "https://yourshop.com/module/aiseomodule/cron?token=YOUR_TOKEN" > /dev/null 2>&1
```

Big shop? Split it into steps. Huge shop (10k+ products)? Use chunked mode. The module shows you the exact commands.

> **You don't need cron for everyday changes.** Edit a product → module pings search engines instantly. Cron is just the nightly full refresh.

---

## 🤖 AI Content Generator

This is the part that saves you hours. Instead of writing SEO content by hand, it reads your actual database and generates:

- ✅ Store description from your real categories & brands
- ✅ Keywords from top categories + newest products
- ✅ Category FAQs — *"What can I find in Shoes?"* with real product count
- ✅ Product FAQs — *"What is Nike Air Max?"* with real price & description
- ✅ Brand FAQs — *"What Nike products are available?"* with count & price range
- ✅ Price range FAQs with actual min-max from your catalog
- ✅ Freshness dates set automatically
- ✅ Store info pulled from PrestaShop config

Run it after install, after adding products, or anytime. It always pulls fresh data.

---

## 🛡️ Bot control

You decide which AI can access your content:

| Bot | What it does | Default |
|-----|-------------|---------|
| Googlebot | Google Search indexing | ✅ Allow |
| GPTBot | OpenAI training | ✅ Allow |
| ChatGPT-User | ChatGPT live browsing | ✅ Allow |
| ClaudeBot | Anthropic Claude AI | ✅ Allow |
| PerplexityBot | Perplexity AI search | ✅ Allow |
| Applebot | Siri & Safari | ✅ Allow |
| Google-Extended | Gemini AI training | ✅ Allow |
| CCBot | Common Crawl scraper | ❌ Block |
| Bytespider | ByteDance crawler | ❌ Block |

Plus 12 more bots you can toggle on/off individually.

---

## 🌍 Languages

The admin interface is translated into **16 languages**:

🇸🇰 Slovak · 🇨🇿 Czech · 🇩🇪 German · 🇫🇷 French · 🇪🇸 Spanish · 🇮🇹 Italian · 🇵🇹 Portuguese · 🇵🇱 Polish · 🇭🇺 Hungarian · 🇷🇴 Romanian · 🇳🇱 Dutch · 🇸🇪 Swedish · 🇩🇰 Danish · 🇫🇮 Finnish · 🇳🇴 Norwegian · 🇬🇷 Greek

---

## 📁 File structure

```
aiseomodule/
├── aiseomodule.php        ← main module file
├── config.xml
├── logo.png
├── LICENSE
├── README.md
├── controllers/front/     ← cron, AI endpoints
├── translations/          ← 16 language files
└── views/templates/       ← admin templates
```

No database tables. Config stored in a JSON file. Uninstall leaves no traces.

---

## 👤 Author

**Yamiru** (Viktor Vasko)

[![Website](https://img.shields.io/badge/yamiru.com-0F172A?style=flat-square&logo=google-chrome&logoColor=white)](https://yamiru.com)
[![GitHub](https://img.shields.io/badge/GitHub-Yamiru-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/Yamiru)

---

## 📄 License

Yamiru Commercial License — see [LICENSE](LICENSE) file.

---

<p align="center">
  <sub>Built with ☕ in Slovakia · Made for PrestaShop · Ready for AI</sub>
</p>
