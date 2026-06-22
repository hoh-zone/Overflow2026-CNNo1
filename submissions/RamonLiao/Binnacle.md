# Binnacle

## Track / 赛道

<!-- 选择一个赛道，把 [ ] 改成 [x] / Select one track -->

- [ ] Agentic Web
- [ ] DeFi & Payments
- [ ] DeepBook
- [x] Walrus

## Description / 项目简介

<!-- 一段话描述你的项目：做什么，为什么重要 / What it does, why it matters -->

*   **Business Pain Points**: Global regulatory frameworks (such as the EU AI Act or MAS FEAT) are shifting to require verifiable audit logs. Existing SaaS log tools are central/mutable, failing chain-of-custody standards. Additionally, logs must be secured against leaking PII/PHI whilst remaining verifiable.
    *   **Solution**: Binnacle provides a tamper-proof audit memory vault. It encrypts AI agent footprints and financial logs, writing them to Walrus as WORM (Write Once, Read Many) blobs, whilst anchoring hash chains on Sui Move. Decryption is gate-controlled via time-locked Seal keys, allowing query audits via an AI agent.
    *   **Key Features**:
        1. **Immutable Logs on Walrus**: Low-cost, long-term retention of encrypted logs.
        2. **Hash-Chained Receipts**: Anchors sequential receipts on-chain, forming a tamper-evident audit track.
        3. **Selective Disclosure via Seal**: Only decrypts logs specified within time-bounded, customer-signed engagements.
        4. **Conversational Audit Agent**: Auditor queries are resolved using MemWal semantic search.

## Links / 链接

- DeepSurge: https://deepsurge.io/... (项目展示页 / Project showcase)
- GitHub: https://github.com/RamonLiao/Binnacle
- Demo Video: https://... (YouTube, ≤ 5 min)
- Website: https://... (optional)

## Team / 团队成员

<!-- 列出所有成员 of GitHub ID / List all team members' GitHub IDs -->

- @RamonLiao

## Deployment / 部署信息

<!-- 填写部署环境和合约地址 / Fill in deployment env and package ID -->

- Env: Testnet
- Package ID: `0x45fccc90178545119c7c578998e86ffc4d1151ddc884524e6b97d39e99d15a6b`

## Swag / 周边

<!-- 如需接收周边，勾选即可，收件信息请通过表单提交（见 guide.md）/ Check if you want swag, submit shipping info via the form -->

- [ ] 我希望接收周边 / I'd like to receive swag
