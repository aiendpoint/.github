# AIEndpoint — The `/ai` Standard

**The web was built for human browsers. AI agents are a fundamentally different client.**

```
AI agent reads a webpage  →  ~50,000 tokens  (95% noise)
AI agent reads /ai        →     ~800 tokens  (0% noise)
```

Any service that exposes `GET /ai` returns a compact JSON description of its capabilities.
AI agents read it directly — no scraping, no guessing, no wasted tokens.

---

### The convention

```
robots.txt   (1994)  →  tells crawlers what NOT to do
sitemap.xml  (2005)  →  tells crawlers where pages are
/ai          (2025)  →  tells AI agents what you CAN DO  ← this
```

It spread without standards committees. It spread without legislation.
Just a useful convention, at a predictable URL.

---

### Try it

```bash
# See a live /ai endpoint
curl https://weather.demo.aiendpoint.dev/ai

# Search the registry from Claude or Cursor
npx -y @aiendpoint/mcp-server

# Add /ai to your own service (Claude Code)
npx skills add aiendpoint/platform --skill aiendpoint
```

---

### Resources

| | |
|---|---|
| 🌐 Website | [aiendpoint.dev](https://aiendpoint.dev) |
| 📖 Why this exists | [aiendpoint.dev/why](https://aiendpoint.dev/why) |
| 📄 Spec | [aiendpoint.dev/docs](https://aiendpoint.dev/docs) |
| ✅ Validator | [aiendpoint.dev/validate](https://aiendpoint.dev/validate) |
| 📦 MCP Server | [@aiendpoint/mcp-server](https://www.npmjs.com/package/@aiendpoint/mcp-server) |

**Open spec · Apache 2.0 · No vendor lock-in**
