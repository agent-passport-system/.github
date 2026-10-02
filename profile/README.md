# Agent Passport System

APS is an open protocol and tools for agents acting on behalf of people and organizations. It combines cryptographic identity, scoped delegation and signed evidence, with enforcement at the boundaries where APS checks are integrated.

Apache-2.0. The specification is the IETF Internet-Draft [draft-pidlisnyi-aps](https://datatracker.ietf.org/doc/draft-pidlisnyi-aps/). Site: [agent-passport.org](https://agent-passport.org).

## Start here

| | |
|---|---|
| TypeScript SDK | [agent-passport-system](https://github.com/agent-passport-system/agent-passport-system) · `npm install agent-passport-system` |
| Python SDK | [agent-passport-python](https://github.com/agent-passport-system/agent-passport-python) · `pip install agent-passport-system` |
| MCP server | [agent-passport-mcp](https://github.com/agent-passport-system/agent-passport-mcp) · `npx agent-passport-system-mcp` |
| Gateway | [agent-passport-gateway](https://github.com/agent-passport-system/agent-passport-gateway), evaluates a requested action against the delegation chain, revocation state and policy, and returns permit or deny with optional signed evidence |

## Verifiers in other languages

[agent-passport-go](https://github.com/agent-passport-system/agent-passport-go) and [agent-passport-rust](https://github.com/agent-passport-system/agent-passport-rust) verify APS artifacts without the TypeScript stack.

## Integrations

Reference implementations, demos and interoperability work.

- [aps-openshell-reference-middleware](https://github.com/agent-passport-system/aps-openshell-reference-middleware): ancestor revocation checks before upstream HTTP dispatch, on the tested relay path
- [aps-1password-demo](https://github.com/agent-passport-system/aps-1password-demo): a runtime key held in 1Password, with APS authority checks at the integrated execution boundary
- [aps-clickhouse-receipts](https://github.com/agent-passport-system/aps-clickhouse-receipts) and [aps-clickhouse-mcp-delegation](https://github.com/agent-passport-system/aps-clickhouse-mcp-delegation): receipts and delegation next to ClickHouse
- [aps-x402-composition](https://github.com/agent-passport-system/aps-x402-composition): delegation and receipts around x402 payment
- [openclaw-plugin-aps](https://github.com/agent-passport-system/openclaw-plugin-aps): OpenClaw plugin
- [aps-sint-interop](https://github.com/agent-passport-system/aps-sint-interop): interop notes with the SINT protocol

## Research

[agent-authority-lifecycle](https://github.com/agent-passport-system/agent-authority-lifecycle): what happens to an agent's authority when people, keys, approvals and roles change around it.

## Shared work outside this org

- [Agent Governance Vocabulary](https://github.com/aeoess/agent-governance-vocabulary): shared terms across agent governance projects
- [Agent Authority Conformance](https://github.com/Agent-Authority-Conformance): a conformance lab approved by LF Decentralized Trust

## What APS does not do

It does not decide whether an action is a good idea. It records the claimed authority and the check result. A receipt says what it proves and what it does not.

Maintained by Tymofii Pidlisnyi ([@aeoess](https://github.com/aeoess)). Contributions are welcome.
