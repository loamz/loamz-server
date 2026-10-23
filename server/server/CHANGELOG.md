# Changelog

## [0.1.1](https://github.com/loamz/loamz-server/compare/loamz-server-v0.1.0...loamz-server-v0.1.1) (2026-10-23)


### Features

* **agents:** tool servers (MCP) for agents, with per-agent tool lists and durable approval of risky calls ([9e8b7a3](https://github.com/loamz/loamz-server/commit/9e8b7a3704e1e54c16dbf4f5593f371eb2eba427))
* **data:** legal holds block erasure, snapshot expiry and history purge ([8302d9e](https://github.com/loamz/loamz-server/commit/8302d9eb6b2cc7ebb8669d49edcb094be49d6af9))
* **data:** personal access tokens with expiry, rotation, revocation and audit ([ef89858](https://github.com/loamz/loamz-server/commit/ef89858b9d3b00e02ed59c9b46e0f0893564ea02))
* **data:** SCIM 2.0 user and group provisioning through Keycloak; chart gives Keycloak the membership secret ([01e4697](https://github.com/loamz/loamz-server/commit/01e46973113c9f619ed611fd9904b35941a8bda9))
* **deploy:** customer-managed encryption keys on AWS, Google Cloud and Azure ([6a7d6bb](https://github.com/loamz/loamz-server/commit/6a7d6bbf0cb619d8bce144336dc8900b658c4339))
* **deploy:** dedicated least-privilege directory client for SCIM; SCIM and access tokens in the end-to-end test ([8be957e](https://github.com/loamz/loamz-server/commit/8be957e3f1ddd019d8296af026d422cf61e87b48))
* **server:** Prometheus metrics at /metrics on both servers; chart ServiceMonitor, alerts and scrape policy ([a7e05d1](https://github.com/loamz/loamz-server/commit/a7e05d1b6ab5bf258c961d193420d10ca44a5946))


### Bug Fixes

* **agents:** one actor per conversation, so concurrent chats no longer fold into each other; e2e covers tool servers, approvals, isolation and overlap ([f995c58](https://github.com/loamz/loamz-server/commit/f995c588c42a6969fcdfdf935a43ab08bd88268a))


### Documentation

* **compliance:** SOC 2 and ISO 27001 control mappings, incident response, vulnerability management, penetration-test scope, trust center, support policy; security.txt; --version ([0c0a263](https://github.com/loamz/loamz-server/commit/0c0a263424d242b0795324677ba0e670ba017b9e))
