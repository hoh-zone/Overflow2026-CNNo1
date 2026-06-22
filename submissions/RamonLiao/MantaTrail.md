# MantaTrail

## Track / 赛道

<!-- 选择一个赛道，把 [ ] 改成 [x] / Select one track -->

- [ ] Agentic Web
- [ ] DeFi & Payments
- [ ] DeepBook
- [x] Walrus

## Description / 项目简介

<!-- 一段话描述你的项目：做什么，为什么重要 / What it does, why it matters -->

*   **Business Pain Points**: Backtest fraud is rampant in quant funds; managers present cherry-picked, overfitted results to investors with no proof of dataset/code authenticity. Additionally, proprietary research libraries, datasets, and training runs evaporate when researchers depart.
    *   **Solution**: MantaTrail establishes a cryptographic audit trail for the quantitative lifecycle. Large tick datasets, strategy code, model weights, and P&L results are stored on Walrus, with parent-child lineage relationships anchored on Sui as a Directed Acyclic Graph (DAG). An off-chain four-agent loop automates the lifecycle from strategy generation to audit minting.
    *   **Key Features**:
        1. **Walrus Artifact Storage**: Content-addressed, cost-effective storage for neural network weights and tick datasets.
        2. **On-Chain Lineage DAG**: Sui Move objects track strategy development edges and dependencies.
        3. **Multi-Agent Quant Loop**: Four agents (Researcher, Backtester, Reviewer, Compliance) run autonomous sandboxed backtesting.
        4. **IP Protection via Seal**: Encrypts trading strategies on Walrus whilst leaving the lineage DAG publicly auditable.

## Links / 链接

- DeepSurge: https://deepsurge.io/... (项目展示页 / Project showcase)
- GitHub: https://github.com/RamonLiao/MantaTrail
- Demo Video: https://... (YouTube, ≤ 5 min)
- Website: https://... (optional)

## Team / 团队成员

<!-- 列出所有成员 of GitHub ID / List all team members' GitHub IDs -->

- @RamonLiao

## Deployment / 部署信息

<!-- 填写部署环境和合约地址 / Fill in deployment env and package ID -->

- Env: Testnet
- Package ID: `0x94b76fce8dd2465a04d927074b96dd61d3973adeaefe99bb8d53150b36f9b3b3`

## Swag / 周边

<!-- 如需接收周边，勾选即可，收件信息请通过表单提交（见 guide.md）/ Check if you want swag, submit shipping info via the form -->

- [ ] 我希望接收周边 / I'd like to receive swag
