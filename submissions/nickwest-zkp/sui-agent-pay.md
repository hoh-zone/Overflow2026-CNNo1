# SuiAgentPay

## Track / 赛道

- [ ] Agentic Web
- [x] DeFi & Payments
- [ ] DeepBook
- [ ] Walrus

## Description / 项目简介

Sui Agent Pay is a demo for an agent-native wallet on Sui. It lets a user create a vault, authorize a time-limited session key, sync that key into a local agent runtime, and then allow an agent to execute wallet actions from natural-language instructions.
The project focuses on a practical control flow for agent spending rather than a generic wallet UI. A session key can execute direct SUI transfers, DeepBook swaps, and whitelisted contract calls. 
Transactions outside the whitelist or above the configured approval threshold trigger a human approval flow through Telegram before execution continues.
The system is built around three layers of control. On-chain, the vault enforces session-key registration, limits, revocation, and expiry. In the runtime, a policy engine applies budget, expiry, and approval rules before execution. On the frontend, the dashboard acts as the operator console for configuring agents, binding Telegram approvals, managing contract whitelists, and monitoring runtime activity.
The latest version also includes session lifecycle handling. When a session key expires, the runtime blocks further execution, surfaces the expired state in the dashboard, supports asset recovery from the session-key address back to the user wallet, and provides a path to revoke the old key and rotate to a new one.
In short, this demo shows the core agent-wallet workflow: controlled delegation, limited permissions, optional human approval, and recoverable session-key operations, all tied together in a minimal end-to-end Sui experience.

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/aa5f388e-b892-4cfc-b0b8-e522acb47538
- GitHub: https://github.com/nickwest-zkp/sui-agent-pay
- Demo Video: https://sui-agent-pay.vercel.app/
- Website: https://sui-agent-pay.vercel.app/

## Team / 团队成员

- @nickwest-zkp

## Deployment / 部署信息

- Env: Testnet
- Package ID: 0xebb525a4dbc110a2329b691adc539ff334cf4b858cccc7f98a2d970b7b56b387

## Swag / 周边

- [X] 我希望接收周边 / I'd like to receive swag
