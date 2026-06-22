# KelpChronicle

## Track / 赛道

<!-- 选择一个赛道，把 [ ] 改成 [x] / Select one track -->

- [ ] Agentic Web
- [ ] DeFi & Payments
- [ ] DeepBook
- [x] Walrus

## Description / 项目简介

<!-- 一段话描述你的项目：做什么，为什么重要 / What it does, why it matters -->

*   **Business Pain Points**: Autonomous AI research agents typically suffer from statelessness or platform lock-in. Their memory databases are centralised under Web2 APIs, transient across sessions, and unverifiable, meaning operators cannot prove their knowledge base has not been poisoned.
    *   **Solution**: KelpChronicle uses Walrus as a persistent, verifiable memory layer and Sui as an integrity anchor. On each run, the agent pulls its memory delta, crawls ecosystem info, compiles findings onto Walrus, and signs the state hash onto Sui Move, making the agent's memory completely portable.
    *   **Key Features**:
        1. **Organic Memory delta**: Agent fetches memory logs from Walrus (MemWal) and appends new research nodes.
        2. **recall Move Attestation**: Anchors memory tree hashes on-chain to guarantee zero data poisoning.
        3. **State Portability**: No platform lock-in; backend states can be restored on any hardware.
        4. **Kelp Forest Graph**: Interactive React UI visualising agent memory nodes as an organic growing graph.

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/1012f704-cf09-4e75-8c81-a7866f41a769
- GitHub: https://github.com/RamonLiao/KelpChronicle
- Demo Video: https://... (YouTube, ≤ 5 min)
- Website: https://... (optional)

## Team / 团队成员

<!-- 列出所有成员 of GitHub ID / List all team members' GitHub IDs -->

- @RamonLiao

## Deployment / 部署信息

<!-- 填写部署环境和合约地址 / Fill in deployment env and package ID -->

- Env: Testnet
- Package ID: `0xcf6ad755a1cdff7217865c796778fabe5aa399cb0cf2eba986f4b582047229c6`

## Swag / 周边

<!-- 如需接收周边，勾选即可，收件信息请通过表单提交（见 guide.md）/ Check if you want swag, submit shipping info via the form -->

- [ ] 我希望接收周边 / I'd like to receive swag
