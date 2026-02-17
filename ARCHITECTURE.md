# Architecture

## Purpose

Hyperledger FireFly is the first open source Supernode: a complete stack for enterprises to build and scale secure Web3 applications. The FireFly API for digital assets, data flows, and blockchain transactions makes it radically faster to build production-ready apps on popular chains and protocols.

## Portfolio role

- Category: External references and mirrors
- Namespace policy: legacy/external
- Repository: https://github.com/Tesseras-Labs/firefly

## Observed baseline signals

- CI workflow present: yes
- Test signal present: yes
- Detected stack:
- Go
- Docker
- GitHub Actions
- Solidity

## Baseline boundaries

- Define external contracts before internal abstractions.
- Keep state transitions explicit and auditable.
- Prefer additive changes and clear rollback paths.

## Immediate next steps

1. Replace placeholder architecture assumptions with concrete runtime and data-flow diagrams.
2. Document integration contracts and failure modes.
3. Link production runbooks and ownership records once assigned.

## Repository review (2026-02-17)

### Evidence reviewed

- Tracked files: 1664
- Detected stack signals: Go,Solidity,Docker
- CI workflows detected: yes
- Test signal detected: yes

### Code surface snapshot

- Top-level code/module directories: cmd/,internal/
- Likely runtime entrypoints: main.go,Dockerfile,Makefile,cmd/version.go,cmd/firefly.go,cmd/firefly_test.go,cmd/version_test.go

### Architecture callouts

Strengths:
- CI workflow files are present under .github/workflows.
- Test-related files or test directory signals are present.
- Repository has non-trivial tracked code/config surface (1664 files).
- Code boundaries are partially explicit via top-level module directories.

Gaps and risks:
- No critical architecture hygiene gap detected from static repository signals.
Recommended next step:
- Publish a concrete runtime/data-flow diagram that maps entrypoints to persistence and external dependencies.
