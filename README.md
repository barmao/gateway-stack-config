# gateway-stack-config — ARCHIVED

> ⚠️ **No longer used.** The Config Server switched from a Git backend to a
> **JDBC/Postgres backend**. Configuration now lives in the `PROPERTIES` table in
> `configdb`, seeded from `infra/postgres/config/config-properties.sql` in the
> main `gateway-stack` repo.
>
> To change config: edit that SQL file and run
> `infra/postgres/setup-configdb.sh` (config-as-code). This repo is kept for
> historical reference only.

---

Previously: externalized non-secret config served by Spring Cloud Config Server
via its Git backend (`application-<env>.yml`, `<service>.yml`).
