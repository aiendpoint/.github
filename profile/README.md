# AIEndpoint

**The `/ai` endpoint standard — make your service instantly readable by AI agents.**

```
robots.txt  →  tells crawlers what NOT to do
sitemap.xml →  tells crawlers where pages are
/ai         →  tells AI agents what you CAN DO
```

Any service that exposes `GET /ai` returns a structured JSON description of its capabilities. AI agents query it directly — no scraping, no documentation parsing, no wasted tokens.

---

### Try it

```bash
curl https://weather.demo.aiendpoint.dev/ai
```

```bash
# Search the registry from Claude or Cursor
npx -y @aiendpoint/mcp-server

# Add /ai to your own service
npx skills add aiendpoint/platform --skill aiendpoint
```

---

### Resources

| | |
|---|---|
| 🌐 Registry | [aiendpoint.dev](https://aiendpoint.dev) |
| 📄 Spec | [spec/v1/schema.json](https://github.com/aiendpoint/platform/blob/main/spec/v1/schema.json) |
| ✅ Validator | [aiendpoint.dev/validate](https://aiendpoint.dev/validate) |
| 📦 MCP Server | [@aiendpoint/mcp-server](https://www.npmjs.com/package/@aiendpoint/mcp-server) |

**Spec is open source · Apache 2.0**
