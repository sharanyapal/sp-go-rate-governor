# Go / Multi-Tenant Rate Governor

### Understand backpressure and throughput through Go concurrency.

**Go** &nbsp;·&nbsp; **Engineering lab** &nbsp;·&nbsp; **Inspect, run, learn**

---

## Why this project matters

Thread-safe per-tenant token bucket with injectable clock, burst capacity, fractional refill and idle-key cleanup.

The repository is intentionally small enough to read through, with the runtime behavior and design choices visible in the source files.

## Getting started

```bash
go test ./...
go run .
```

## Read the implementation

| Path | Role |
|--|--|
| [`README.md`](./README.md) | Background and documentation |
| [`go.mod`](./go.mod) | Go module metadata |

## A good way to explore it

1. Run the example using the instructions above.
2. Change a controlled input or simulated condition.
3. Compare what you observe with the source and existing tests.

## Scope

This is an illustrative, local engineering project rather than an independently audited production service. Synthetic data and test scenarios are for learning; do not rely on them for real-world operational guarantees.

<details>
<summary><strong>Detailed original notes and commands</strong></summary>

# Go / Multi-Tenant Rate Governor

Thread-safe per-tenant token bucket with injectable clock, burst capacity, fractional refill and idle-key cleanup.

```bash
go test -race ./...
```

Ideal for API gateways and IAM login throttling. In-memory demo only; distributed quotas need Redis/atomic counters.

</details>

---

<sub>From [Sharanya Pal's engineering projects](https://github.com/sharanyapal?tab=repositories).</sub>
