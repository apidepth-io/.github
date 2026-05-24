# Apidepth

**API dependency monitoring for developers.**

Know when your third-party APIs are slow, rate-limiting, or failing — before your users do. Apidepth sits inside your existing HTTP client and reports latency, errors, and rate limit burn-down automatically.

---

## SDKs

| Language | Install |
|---|---|
| **Ruby** | `gem install apidepth` |
| **Python** | `pip install apidepth` |
| **JavaScript / TypeScript** | `npm install apidepth` |

### Quick start (Node.js)

```ts
import { instrument } from "apidepth";

instrument({ apiKey: "apd_live_..." });

// Your existing fetch/axios/got calls are now tracked automatically
const res = await fetch("https://api.stripe.com/v1/charges");
```

---

## What gets tracked

- **Latency** — p50/p95/p99 per vendor and endpoint
- **Errors** — 4xx/5xx rates with outcome classification
- **Rate limits** — 429 tracking and burn-down prediction
- **Fleet benchmarks** — how your latency compares to other Apidepth users hitting the same API
- **Probe monitoring** — active uptime checks with incident and TLS expiry alerts

---

## Repos

| Repo | Description |
|---|---|
| [apidepth-ruby](https://github.com/apidepth-io/apidepth-ruby) | Ruby gem |
| [apidepth-python](https://github.com/apidepth-io/apidepth-python) | Python SDK |
| [apidepth-javascript](https://github.com/apidepth-io/apidepth-javascript) | JavaScript / TypeScript SDK |

---

[apidepth.io](https://apidepth.io)
