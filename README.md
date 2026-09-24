# Vidu Q3 API (viduq3) — api guide with published pricing

> **540P $0.04; default $0.08; 720P $0.08** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-e37d66)** · **[Get an API key](https://go.apimart.ai/k-4424d6)**

Everything here refers to **viduq3** — also written **viduq3** or **viduq3**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `540P` | $0.04 |
| `default` | $0.08 |
| `720P` | $0.08 |
| `1080P` | $0.1 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $4 |
| 1,000 | $40 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/videos/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"viduq3","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
