# Gyre Vault

## Track / 赛道

<!-- 选择一个赛道，把 [ ] 改成 [x] / Select one track -->

- [ ] Agentic Web
- [ ] DeFi & Payments
- [x] DeepBook
- [ ] Walrus

## Description / 项目简介

<!-- 一段话描述你的项目：做什么，为什么重要 / What it does, why it matters -->

*   **Business Pain Points**: While Sui promotes atomic composability, DeFi TVL remains siloed, forcing LPs to choose between low LST yields (~4%) or highly manual option writing. EVM equivalents require custom callback adapter contracts, adding massive audit overhead.
    *   **Solution**: Gyre is a structured yield vault that stacks three distinct protocols in a single PTB. It lends LSTs to Iron Bank, borrows dUSDC from DeepBook Margin using the lending receipt as collateral, and deploys dUSDC into DeepBook Predict to capture range premia.
    *   **Key Features**:
        1. **Leveraged Yield Loop**: Single-signature PTB orchestrating lending, borrowing, and options writing.
        2. **Option-Bounded LTV**: Calculates LTV boundaries against the option's worst-case payout floor to prevent liquidation cascades.
        3. **Auto-Deleveraging & Rolling**: Keeper automatically rolls expiries and executes partial unwinds if price approaches boundaries.
        4. **vGyre Tokenisation**: Mints yield-bearing shares for LP liquidity.

## Links / 链接

- DeepSurge: https://deepsurge.io/... (项目展示页 / Project showcase)
- GitHub: https://github.com/RamonLiao/Gyre
- Demo Video: https://... (YouTube, ≤ 5 min)
- Website: https://... (optional)

## Team / 团队成员

<!-- 列出所有成员 of GitHub ID / List all team members' GitHub IDs -->

- @RamonLiao

## Deployment / 部署信息

<!-- 填写部署环境和合约地址 / Fill in deployment env and package ID -->

- Env: Testnet
- Package ID: `0xd6a42f4df4db73d68cbeb52be66698d2fe6a9464f45ad113ca52b0c6ebd918b6`

## Swag / 周边

<!-- 如需接收周边，勾选即可，收件信息请通过表单提交（见 guide.md）/ Check if you want swag, submit shipping info via the form -->

- [ ] 我希望接收周边 / I'd like to receive swag
