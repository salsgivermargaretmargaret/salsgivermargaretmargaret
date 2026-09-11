I build low-latency payment APIs and the event-driven systems that keep them reliable.
## @salsgivermargaretmargaret
I own payment APIs, queue consumers, schema contracts, and deployment workflows.
I have built idempotent workers, typed RPCs, and migration tooling for systems where partial failure is routine.
Operational clarity matters more to me than architectural novelty.
I accept a little duplication when it keeps ownership and recovery paths obvious.
### 🛠 Tech & Infrastructure
- **Core:** TypeScript, NestJS, Prisma, Redis
- **Data:** PostgreSQL, ClickHouse, Kafka
- **Infra:** Docker, Kubernetes, Terraform
- **Tooling:** Jest, OpenTelemetry
### ⚙️ Engineering Areas
- Idempotent payment APIs with stable request IDs and bounded retry budgets.
- Kafka consumer groups with schema evolution and replay-safe processing.
- PostgreSQL migrations with reversible changes and index-health checks.
- Distributed tracing across APIs, queues, workers, and downstream providers.
### 🔭 Current Focus
- Reducing retry amplification without dropping payments that arrive during provider outages.
- Separating durable ledger state from display-only aggregates without adding a synchronous dependency.
- Tightening schema compatibility so older consumers can read new event fields.
- Cutting queue replay time while preserving exactly-once business effects.
### 📌 Engineering Notes
- Tests should cover contract boundaries, not just happy-path function calls.
- Boundaries need explicit ownership, validation, and failure semantics.
- Migrations belong with the code that reads and writes them.
- Retries need limits, jitter, and a recorded reason for each attempt.
### 🧭 How I Work
- Prefer boring, observable primitives over custom coordination code.
- Keep failure paths and recovery paths testable from the first implementation.
- Make trade-offs visible in the code, diagrams, and runbooks.
*Reliable systems are made of small, reviewable decisions.*
[Email](mailto:salsgivermargaretmargaret@gmail.com)