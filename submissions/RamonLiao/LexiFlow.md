# LexiFlow

## Track / 赛道

<!-- 选择一个赛道，把 [ ] 改成 [x] / Select one track -->

- [x] Agentic Web
- [ ] DeFi & Payments
- [ ] DeepBook
- [ ] Walrus

## Description / 项目简介

<!-- 一段话描述你的项目：做什么，为什么重要 / What it does, why it matters -->

*   **Business Pain Points**: DeFi user experiences are notoriously complex. Users face opaque transaction signatures (raw hex or unparsed Move structures), leading to blind-signing (nearly 95% of users blind-sign, causing millions in exploit losses). Furthermore, relying solely on LLMs to generate transactions is highly dangerous due to potential hallucinations.
    *   **Solution**: LexiFlow compiles natural-language commands (e.g. "move my idle USDC from Scallop to Navi") into secure, atomic Sui PTBs. It simulates proposed transactions in a local sandbox to inspect them against strict safety policies and presents the user with a plain-English risk card prior to zkLogin signature execution.
    *   **Key Features**:
        1. **Natural-Language to PTB Compiler**: Converts user statements into multi-protocol atomic transaction blocks.
        2. **Deterministic Guardian Layer**: Inspects PTBs for stale oracle feeds (>60s), thin liquidity pools, and fee anomalies.
        3. **zkLogin Integration**: Eliminates seed phrase friction via Google/Apple OAuth onboarding.
        4. **White-Label SDK**: Enables Web2 platforms to integrate secure stablecoin and yield settlement with a single line of code.

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/3ce06a89-0e9f-4342-99ac-dec67460165f
- GitHub: https://github.com/RamonLiao/LexiFlow
- Demo Video: https://... (YouTube, ≤ 5 min)
- Website: https://... (optional)

## Team / 团队成员

<!-- 列出所有成员 of GitHub ID / List all team members' GitHub IDs -->

- @RamonLiao

## Deployment / 部署信息

<!-- 填写部署环境和合约地址 / Fill in deployment env and package ID -->

- Env: Testnet
- Package ID: `0xb7b60859f62d81384b49bfc3a166c1907ad1798cf37cf3f100bff3c4164f07b7`

## Swag / 周边

<!-- 如需接收周边，勾选即可，收件信息请通过表单提交（见 guide.md）/ Check if you want swag, submit shipping info via the form -->

- [ ] 我希望接收周边 / I'd like to receive swag
