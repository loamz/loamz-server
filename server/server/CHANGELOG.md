# Changelog

## [0.1.1](https://github.com/loamz/loamz-server/compare/loamz-server-v0.1.0...loamz-server-v0.1.1) (2026-10-27)


### Features

* a development mode for the cell, and code-interpreter files that show in the chat ([814d855](https://github.com/loamz/loamz-server/commit/814d8550079e75e21dc275eaeb6012b92d0d5148))
* **agents:** a data_chart tool that draws a query result as a chart ([e650af9](https://github.com/loamz/loamz-server/commit/e650af9500588ebc09027cd2d3c58a80ca17e2c6))
* **agents:** data tools (search, describe, SQL) that query as the signed-in person and their teams ([5f14693](https://github.com/loamz/loamz-server/commit/5f146936698b193dabef77f311746112b4a98df5))
* **agents:** hosted agents can use the code interpreter, with governed data ([a9c146c](https://github.com/loamz/loamz-server/commit/a9c146cca7967929eed774a13bfaf67970dfb1df))
* **agents:** the sandbox holds no data credential; one gateway socket per run, with the run's person and teams, and a byte budget ([e81cdaf](https://github.com/loamz/loamz-server/commit/e81cdafb771c10c75a5f799b7bbc047b09e848e2))
* **agents:** tool servers (MCP) for agents, with per-agent tool lists and durable approval of risky calls ([9e8b7a3](https://github.com/loamz/loamz-server/commit/9e8b7a3704e1e54c16dbf4f5593f371eb2eba427))
* **console:** rich pages from the model, drawn with OpenUI's component library ([3442587](https://github.com/loamz/loamz-server/commit/3442587565a35fca5970fff8bbec32e00bcf15a6))
* **console:** tools and agents can draw UI in a message, in the json-render standard ([d49558c](https://github.com/loamz/loamz-server/commit/d49558c00f3013eefd11998a2e5d837dcd8c7126))
* **console:** UI in a message is A2UI ([602fac9](https://github.com/loamz/loamz-server/commit/602fac97b10651b5336f878b001027e9559cdea6))
* **data:** legal holds block erasure, snapshot expiry and history purge ([8302d9e](https://github.com/loamz/loamz-server/commit/8302d9eb6b2cc7ebb8669d49edcb094be49d6af9))
* **data:** personal access tokens with expiry, rotation, revocation and audit ([ef89858](https://github.com/loamz/loamz-server/commit/ef89858b9d3b00e02ed59c9b46e0f0893564ea02))
* **data:** SCIM 2.0 user and group provisioning through Keycloak; chart gives Keycloak the membership secret ([01e4697](https://github.com/loamz/loamz-server/commit/01e46973113c9f619ed611fd9904b35941a8bda9))
* **deploy:** customer-managed encryption keys on AWS, Google Cloud and Azure ([6a7d6bb](https://github.com/loamz/loamz-server/commit/6a7d6bbf0cb619d8bce144336dc8900b658c4339))
* **deploy:** dedicated least-privilege directory client for SCIM; SCIM and access tokens in the end-to-end test ([8be957e](https://github.com/loamz/loamz-server/commit/8be957e3f1ddd019d8296af026d422cf61e87b48))
* **messenger:** people and agents in shared chats, a live feed, push and a nonce CSP (Phase 0, first part) ([634f378](https://github.com/loamz/loamz-server/commit/634f378e8e08fb891ae947baa097ef027a8a7215))
* **messenger:** typing, receipts, sealing at rest, an XSS corpus, and verified two-user chat (Phase 0 and S, second part) ([7eaba56](https://github.com/loamz/loamz-server/commit/7eaba56e2e524eb3e2c1f2072bef57d82b56f96e))
* one bubble per turn, A2UI in groups, and web pictures through a safe proxy ([f63c446](https://github.com/loamz/loamz-server/commit/f63c4466999a81616371ebb69577e2d7ecdd2805))
* **server:** Prometheus metrics at /metrics on both servers; chart ServiceMonitor, alerts and scrape policy ([a7e05d1](https://github.com/loamz/loamz-server/commit/a7e05d1b6ab5bf258c961d193420d10ca44a5946))


### Bug Fixes

* **agents:** one actor per conversation, so concurrent chats no longer fold into each other; e2e covers tool servers, approvals, isolation and overlap ([f995c58](https://github.com/loamz/loamz-server/commit/f995c588c42a6969fcdfdf935a43ab08bd88268a))
* **chat:** rejoin a run that waits on a person, and clear one that can never continue ([a91c2b3](https://github.com/loamz/loamz-server/commit/a91c2b39035faf7b2fc5e69b1e133482a9edcefd))
* files the agent makes show in the chat; a restart no longer blocks a conversation; no repeated sender name ([2338321](https://github.com/loamz/loamz-server/commit/233832100bb36c9b6bc5f886f71e6704d62683bf))
* **sandbox:** code never runs as root; each run's data socket belongs to the id the code runs as ([ccd7b21](https://github.com/loamz/loamz-server/commit/ccd7b2192dad16b27a091b9efcb8bec6f2bdad89))


### Documentation

* **compliance:** SOC 2 and ISO 27001 control mappings, incident response, vulnerability management, penetration-test scope, trust center, support policy; security.txt; --version ([0c0a263](https://github.com/loamz/loamz-server/commit/0c0a263424d242b0795324677ba0e670ba017b9e))
