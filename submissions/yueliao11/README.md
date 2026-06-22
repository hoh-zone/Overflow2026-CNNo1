# MemTube

## Track / 赛道

- [x] Walrus

## Description / 项目简介

MemTube is an on-chain AI video content production platform built on Sui and Walrus. It enables creators to register a Channel with a persistent memory manifest stored on Walrus, launch production runs where AI agents generate scripts, storyboards, subtitles, and video artifacts, and publish immutable ContentPackages whose blob references are anchored on-chain. Every step — channel creation, run lifecycle transitions (DRAFT → RUNNING → READY → PUBLISHED), and package publishing — is recorded as a Sui object with tamper-evident SHA-256 hashes, making the entire content pipeline auditable and reproducible. The smart contract suite (channel, run, package, access, errors modules) enforces role-based access control and ownership semantics fully on-chain, while the Next.js frontend integrates with @mysten/dapp-kit for seamless wallet connectivity.

### Modules
- `memtube::channel` — Channel identity, memory manifest, collaborator roles
- `memtube::run` — Production run lifecycle state machine
- `memtube::package` — Immutable content package with Walrus blob anchoring
- `memtube::access` — Transferable capability objects for delegation
- `memtube::errors` — Shared error codes

### Tech Stack
- Smart Contracts: Move (Sui 2024 edition), deployed on Sui Testnet
- Storage: Walrus (decentralized blob storage for AI artifacts)
- Frontend: Next.js 13, TypeScript, Tailwind CSS, shadcn/ui
- Wallet: @mysten/dapp-kit (Slush, Sui Wallet compatible)
- Database: Supabase (off-chain metadata indexing)

## Links / 链接
- DeepSurge: https://www.deepsurge.xyz/projects/5dff978d-1db5-4d5d-9091-48a8797cdf63
- GitHub: https://github.com/yueliao11/memtube.git
- Demo Video: https://youtu.be/5d6BljjEQiU
- Website: https://tube.swingforbrainrots.com/

## Team / 团队成员

- @yueliao11

## Deployment / 部署信息

- Env: Testnet
- Package ID: `0x419ae89db372bd7cd2b168ac9b92dff82c0fe302e365c3c317046d65567d7a4c`
- Deployer Address: `0x1c690da1a6fe32c9ba1ca7b85a415c8d22364b55bf8ffcfe06b745c147ff0240`
- Deploy Transaction: `E3YPGMkK6j2uk9xRjuuqguRGkFc9F17YFyWyJHt4FkSm`

## Swag / 周边

- [✓] 我希望接收周边 / I would like to receive swag
