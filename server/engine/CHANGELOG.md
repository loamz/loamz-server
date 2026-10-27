# Changelog

## [0.1.1](https://github.com/loamz/loamz-server/compare/loamz-engine-v0.1.0...loamz-engine-v0.1.1) (2026-10-27)


### Features

* **agents:** a data_chart tool that draws a query result as a chart ([e650af9](https://github.com/loamz/loamz-server/commit/e650af9500588ebc09027cd2d3c58a80ca17e2c6))
* **agents:** data tools (search, describe, SQL) that query as the signed-in person and their teams ([5f14693](https://github.com/loamz/loamz-server/commit/5f146936698b193dabef77f311746112b4a98df5))
* **agents:** hosted agents can use the code interpreter, with governed data ([a9c146c](https://github.com/loamz/loamz-server/commit/a9c146cca7967929eed774a13bfaf67970dfb1df))
* **agents:** the sandbox holds no data credential; one gateway socket per run, with the run's person and teams, and a byte budget ([e81cdaf](https://github.com/loamz/loamz-server/commit/e81cdafb771c10c75a5f799b7bbc047b09e848e2))
* **agents:** tool servers (MCP) for agents, with per-agent tool lists and durable approval of risky calls ([9e8b7a3](https://github.com/loamz/loamz-server/commit/9e8b7a3704e1e54c16dbf4f5593f371eb2eba427))
* **console:** tools and agents can draw UI in a message, in the json-render standard ([d49558c](https://github.com/loamz/loamz-server/commit/d49558c00f3013eefd11998a2e5d837dcd8c7126))
* **data:** legal holds block erasure, snapshot expiry and history purge ([8302d9e](https://github.com/loamz/loamz-server/commit/8302d9eb6b2cc7ebb8669d49edcb094be49d6af9))
* **messenger:** people and agents in shared chats, a live feed, push and a nonce CSP (Phase 0, first part) ([634f378](https://github.com/loamz/loamz-server/commit/634f378e8e08fb891ae947baa097ef027a8a7215))
* **messenger:** typing, receipts, sealing at rest, an XSS corpus, and verified two-user chat (Phase 0 and S, second part) ([7eaba56](https://github.com/loamz/loamz-server/commit/7eaba56e2e524eb3e2c1f2072bef57d82b56f96e))
* one bubble per turn, A2UI in groups, and web pictures through a safe proxy ([f63c446](https://github.com/loamz/loamz-server/commit/f63c4466999a81616371ebb69577e2d7ecdd2805))


### Bug Fixes

* a message shows its chart as it was, even after the agent redraws the file ([9feb074](https://github.com/loamz/loamz-server/commit/9feb0748d3402996c836a251d8ec157de5c34389))
* files the agent makes show in the chat; a restart no longer blocks a conversation; no repeated sender name ([2338321](https://github.com/loamz/loamz-server/commit/233832100bb36c9b6bc5f886f71e6704d62683bf))
* **sandbox:** code never runs as root; each run's data socket belongs to the id the code runs as ([ccd7b21](https://github.com/loamz/loamz-server/commit/ccd7b2192dad16b27a091b9efcb8bec6f2bdad89))
* **tools:** a tool server connection is opened and closed by one owner task; dead servers fail fast and cannot starve or cancel other work ([e1b540b](https://github.com/loamz/loamz-server/commit/e1b540b39ba6f585eae1b927bc070c3f519e2c8c))
