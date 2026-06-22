# TideWard

## Track / 赛道

<!-- 选择一个赛道，把 [ ] 改成 [x] / Select one track -->

- [x] Agentic Web
- [ ] DeFi & Payments
- [ ] DeepBook
- [ ] Walrus

## Description / 项目简介

<!-- 一段话描述你的项目：做什么，为什么重要 / What it does, why it matters -->

*   **Business Pain Points**: DeFi lending and perpetual protocols managing billions in TVL rely on static risk parameters (LTV, borrow caps, interest rates) and slow DAO governance processes. When stablecoins de-peg or oracle prices deviate, markets collapse in seconds, causing millions in bad debt before human governors can react.
    *   **Solution**: TideWard bridges off-chain risk intelligence and on-chain execution. It runs an autonomous risk scoring agent that calculates risk indices in real time and automatically dispatches atomic Programmable Transaction Blocks (PTBs) to adjust parameters on a Sui Move `RiskPolicy` object, whilst preserving a first-class DAO override capability to rollback adjustments.
    *   **Key Features**:
        1. **Autonomous On-Chain Enforcement**: Executes parameter adjustments such as LTV capping and market pausing.
        2. **Move Policy Objects**: VM-level assertion gates checking policy states prior to lending executions.
        3. **First-Class DAO Override**: Single-click rollbacks via the `OverrideCap` held by the DAO multisig.
        4. **Granular Blast Radius**: Policy scoping per pool or market rather than protocol-wide globals.

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/1e4f1f30-e427-4625-a9bd-47d3d7bb841f
- GitHub: https://github.com/RamonLiao/TideWard
- Demo Video: https://... (YouTube, ≤ 5 min)
- Website: https://... (optional)

## Team / 团队成员

<!-- 列出所有成员 of GitHub ID / List all team members' GitHub IDs -->

- @RamonLiao

## Deployment / 部署信息

<!-- 填写部署环境和合约地址 / Fill in deployment env and package ID -->

- Env: Testnet
- Package ID: `0x696e09998424a06317673c742ed54297811ed8d0db0deac269ca56a0a6997fc8`

## Swag / 周边

<!-- 如需接收周边，勾选即可，收件信息请通过表单提交（见 guide.md）/ Check if you want swag, submit shipping info via the form -->

- [ ] 我希望接收周边 / I'd like to receive swag
