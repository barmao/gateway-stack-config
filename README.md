# gateway-stack-config

Externalized **non-secret** configuration served by the Spring Cloud Config
Server. Public on purpose — it contains configuration only.

**Never put secrets here.** DB passwords, tokens, keys live in Vault; the Config
Server merges them in (composite backend).

- `application.yml` — defaults applied to every service
- `<service>.yml` — per-service config (e.g. `orders-api.yml`)
