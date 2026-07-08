## 📌 Featured Project

### 🔗 [PaceDrop](https://github.com/tarunrajpurohit/PaceDrop)

A **multi-channel dropshipping platform** connecting manufacturers and resellers — with automated product sync, inventory management, and an admin-driven import approval workflow, while preserving manufacturer anonymity on reseller-facing endpoints.

**Tech used:**
`Next.js` `Node.js` `TypeScript` `PostgreSQL` `Redis` `BullMQ`

**Highlights:**

- 🔄 **Event-driven backend** — custom distributed EventBus (Redis Pub/Sub + distributed locks) decouples controllers from services, keeping the system safe to scale horizontally
- 🚦 **Background job processing** — BullMQ + Redis handle heavy async work (e.g. Shopify channel sync) without blocking requests
- ⚡ **Cache-aside pattern** — Redis caches product data with automatic invalidation on writes
- 🔐 **Security-first** — AES-256 encrypted tokens, hashed API keys, Zod-validated inputs throughout
- 🧪 **API testing** — Git-friendly, version-controlled contracts via Bruno
