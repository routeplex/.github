<div align="center">

# RoutePlex

**The unified AI gateway for the modern stack.**

[![Website](https://img.shields.io/badge/Website-routeplex.com-6366f1)](https://routeplex.com)
[![Docs](https://img.shields.io/badge/Docs-Getting%20Started-green)](https://routeplex.com/docs)
[![Discord](https://img.shields.io/badge/Discord-Join%20us-5865F2)](https://discord.gg/BaFcXQJA)
[![X](https://img.shields.io/badge/X-@routeplex-000000)](https://x.com/routeplex)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-RoutePlex-0A66C2)](https://www.linkedin.com/company/routeplex)

</div>

---

### What is RoutePlex?

RoutePlex is a unified API gateway that gives you access to **22+ AI models** from OpenAI, Anthropic, and Google through a single endpoint. One API key, one integration, every model.

### Why RoutePlex?

- **Smart Routing** — Automatically route to the best model based on cost, speed, quality, or a balanced trade-off
- **Built-in Failover** — If a provider goes down, requests are automatically rerouted to a fallback model
- **Web-Augmented AI** — Real-time web search and URL fetching are auto-detected and injected into LLM context
- **Content Safety** — Three-layer moderation pipeline screens every request and response
- **OpenAI SDK Compatible** — Drop-in replacement: change the base URL and you're done
- **Cost Governance** — Budgets, usage caps, and per-request cost tracking out of the box

### Repositories

| Repo | Description |
|------|-------------|
| [routeplex-examples](https://github.com/routeplex/routeplex-examples) | Working code examples in Python, JavaScript, TypeScript, and cURL |

### Quick Start

```bash
curl https://api.routeplex.com/api/v1/chat \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{"messages": [{"role": "user", "content": "Hello!"}], "mode": "routeplex-ai", "strategy": "balanced"}'
```

### Links

- [Documentation](https://routeplex.com/docs)
- [API Reference](https://routeplex.com/api-reference)
- [Models](https://routeplex.com/models)
- [Pricing](https://routeplex.com/pricing)
- [Blog](https://routeplex.com/blog)
- [Changelog](https://routeplex.com/changelog)

---

<div align="center">
<sub>Built with care in 2026. <a href="https://routeplex.com">routeplex.com</a></sub>
</div>
