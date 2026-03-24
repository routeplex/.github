<div align="center">

# RoutePlex

**The unified AI gateway for the modern stack.**

[![Website](https://img.shields.io/badge/Website-routeplex.com-6366f1)](https://routeplex.com)
[![Docs](https://img.shields.io/badge/Docs-Getting%20Started-green)](https://routeplex.com/docs)
[![PyPI](https://img.shields.io/pypi/v/routeplex?label=PyPI&color=blue)](https://pypi.org/project/routeplex/)
[![npm](https://img.shields.io/npm/v/@routeplex/node?label=npm&color=red)](https://www.npmjs.com/package/@routeplex/node)
[![Discord](https://img.shields.io/badge/Discord-Join%20us-5865F2)](https://discord.gg/BaFcXQJA)
[![X](https://img.shields.io/badge/X-@routeplex-000000)](https://x.com/routeplex)

</div>

---

### What is RoutePlex?

RoutePlex is a unified API gateway that gives you access to **22+ AI models** from OpenAI, Anthropic, and Google through a single endpoint. One API key, one integration, every model.

### Why RoutePlex?

- **Prompt-Based Auto-Routing** — RoutePlex analyzes your prompt and picks the best model automatically. Or override with a strategy (cost, speed, quality, balanced)
- **Built-in Failover** — If a provider goes down, requests are automatically rerouted to a fallback model
- **Web-Augmented AI** — Real-time web search and URL fetching are auto-detected and injected into LLM context
- **Content Safety** — Three-layer moderation pipeline screens every request and response
- **OpenAI SDK Compatible** — Drop-in replacement: change the base URL and you're done
- **Cost Governance** — Budgets, usage caps, and per-request cost tracking out of the box

### SDKs

```bash
pip install routeplex          # Python
npm install @routeplex/node    # Node.js
```

```python
from routeplex import RoutePlex

client = RoutePlex(api_key="rp_your_key")

# Auto-routing — analyzes your prompt, picks the best model
response = client.chat("Explain quantum computing")
print(response.output)

# Or override with a strategy
response = client.chat("Summarize this article", strategy="cost")
```

```javascript
const { RoutePlex } = require("@routeplex/node");

const client = new RoutePlex({ apiKey: "rp_your_key" });

// Auto-routing — analyzes your prompt, picks the best model
const res = await client.chat("Explain quantum computing");
console.log(res.output);

// Or override with a strategy
const fast = await client.chat("What is 2+2?", { strategy: "speed" });
```

### Repositories

| Repo | Description |
|------|-------------|
| [`routeplex-python`](https://github.com/routeplex/routeplex-python) | Official Python SDK ([PyPI](https://pypi.org/project/routeplex/)) |
| [`routeplex-node`](https://github.com/routeplex/routeplex-node) | Official Node.js SDK ([@routeplex/node](https://www.npmjs.com/package/@routeplex/node)) |
| [`routeplex-examples`](https://github.com/routeplex/routeplex-examples) | Working examples in Python, JS, TypeScript, and cURL |

### Quick Start

```bash
# Auto-routing — RoutePlex analyzes your prompt and picks the best model
curl https://api.routeplex.com/api/v1/chat \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{"messages": [{"role": "user", "content": "Hello!"}], "mode": "routeplex-ai"}'
```

### Links

- [Documentation](https://routeplex.com/docs)
- [API Playground](https://routeplex.com/docs/api-reference/playground)
- [Models](https://routeplex.com/models)
- [Pricing](https://routeplex.com/pricing)
- [Changelog](https://routeplex.com/changelog)

### Contributing

We welcome contributions! See our [Contributing Guide](https://github.com/routeplex/.github/blob/main/CONTRIBUTING.md) for details.

- **Found a bug?** [Open an issue](https://github.com/routeplex/.github/issues) with a reproduction
- **Feature idea?** [Open a feature request](https://github.com/routeplex/.github/issues)
- **Security issue?** Email [security@routeplex.com](mailto:security@routeplex.com) — do not open a public issue

---

<div align="center">
<sub>Built with care in 2026. <a href="https://routeplex.com">routeplex.com</a></sub>
</div>
