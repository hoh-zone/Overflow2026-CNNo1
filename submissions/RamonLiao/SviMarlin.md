# SviMarlin

## Track / 赛道

<!-- 选择一个赛道，把 [ ] 改成 [x] / Select one track -->

- [ ] Agentic Web
- [ ] DeFi & Payments
- [x] DeepBook
- [ ] Walrus

## Description / 项目简介

<!-- 一段话描述你的项目：做什么，为什么重要 / What it does, why it matters -->

*   **Business Pain Points**: Prediction markets have seen explosive growth but remain structurally inefficient. Standard platforms quote simple binary probabilities, failing to price volatility smiles or term structures. This creates significant implied volatility discrepancies (often 20–40 vol points) across fragmented venues.
    *   **Solution**: SviMarlin is a high-performance quant trading engine. It stream-solves the on-chain SVI (Stochastic Volatility Inspired) surface from DeepBook Predict, aggregates prices from external venues (Hyperliquid, Limitless), and executes atomic spread trades on Sui while delta-hedging residual exposure.
    *   **Key Features**:
        1. **Implied Vol Solver**: Back-solves SVI parameters from DeepBook Predict's oracle updates.
        2. **Multi-Venue Pricing Engine**: Translates binary options from multiple venues into implied volatilities.
        3. **Atomic Spread execution**: Mints underpriced binary options on Sui and sells overpriced legs on external venues.
        4. **Risk Mitigator**: Incorporates Kelly sizing, Pyth price verifications, and delta-hedging perp strategies.

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/3ffe2cdb-f54f-40a3-a21e-5a81acef1d1b
- GitHub: https://github.com/RamonLiao/SviMarlin
- Demo Video: https://... (YouTube, ≤ 5 min)
- Website: https://... (optional)

## Team / 团队成员

<!-- 列出所有成员 of GitHub ID / List all team members' GitHub IDs -->

- @RamonLiao

## Deployment / 部署信息

<!-- 填写部署环境和合约地址 / Fill in deployment env and package ID -->

- Env: Testnet
- Package ID: `0x6976a27bcedf6bdb47f6c597e80da0b4526546ad30767e4733cf3a7030373382`

## Swag / 周边

<!-- 如需接收周边，勾选即可，收件信息请通过表单提交（见 guide.md）/ Check if you want swag, submit shipping info via the form -->

- [ ] 我希望接收周边 / I'd like to receive swag
