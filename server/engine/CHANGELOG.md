# Changelog

## [0.1.1](https://github.com/loamz/loamz-server/compare/loamz-engine-v0.1.0...loamz-engine-v0.1.1) (2026-10-23)


### Features

* **agents:** tool servers (MCP) for agents, with per-agent tool lists and durable approval of risky calls ([9e8b7a3](https://github.com/loamz/loamz-server/commit/9e8b7a3704e1e54c16dbf4f5593f371eb2eba427))
* **data:** legal holds block erasure, snapshot expiry and history purge ([8302d9e](https://github.com/loamz/loamz-server/commit/8302d9eb6b2cc7ebb8669d49edcb094be49d6af9))


### Bug Fixes

* **tools:** a tool server connection is opened and closed by one owner task; dead servers fail fast and cannot starve or cancel other work ([e1b540b](https://github.com/loamz/loamz-server/commit/e1b540b39ba6f585eae1b927bc070c3f519e2c8c))
