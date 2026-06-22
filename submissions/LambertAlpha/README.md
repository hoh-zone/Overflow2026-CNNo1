# LadderVault

> **Active risk-managed LP vault for DeepBook Predict.** A quant concentration signal cuts worst-case LP drawdown by 82% — no directional bets. Live on Sui testnet with real end-to-end transactions.
> **DeepBook Predict 上的主动风险管理 LP 金库**:用量化集中度信号把 LP 最坏回撤削掉 82%,不赌方向。已部署 Sui testnet,链上端到端交易跑通。

## Track / 赛道

- [ ] Agentic Web
- [ ] DeFi & Payments
- [x] **DeepBook**
- [ ] Walrus

## Description / 项目简介

**Problem.** Passive LPs in prediction markets earn making fees but are *passive*: when traders concentrate positions on a hot strike and price pins there, those positions settle in-the-money together and the LP eats an asymmetric tail loss it cannot dodge.

**Solution.** LadderVault is an actively risk-managed LP vault. It monitors a **concentration signal** — `pin_risk` = payout at the current price / total inventory — and **automatically withdraws** liquidity from Predict when concentration spikes, re-entering (with hysteresis) once it subsides.

**Verified result — reproducible, not a claim.** In a faithful offline kill-test, the worst-case (price-pinned) scenario takes a **passive LP to -13.4%**, while the concentration-driven active strategy holds it at **-0.1% — an 82% tail reduction that approaches a look-ahead Oracle upper bound**. Reproduce in one command: `cd research && uv run python run_killtest.py`. Methodology and every assumption/limitation are written out in `docs/kill-test-design.md`.

**Why this is real, not a mockup.** (1) Move contracts **deployed to Sui testnet** (package ID below, Explorer-verifiable). (2) A **real end-to-end on-chain transaction** runs the full story in one PTB: deposit -> traders push concentration to 80% -> vault auto-exits. (3) **Two Move unit tests pass**, covering the full lifecycle (deposit -> spike -> exit -> settlement-the-vault-dodged -> re-enter -> redeem >= principal). (4) The quant result is **reproducible from source**.

**Sui integration depth.** Move **shared-object** vault + an `LV` share token minted/burned by NAV + **PTB-composed** `deposit`/`withdraw`/`rebalance`, with the LP interface **aligned to DeepBook Predict's `supply`/`withdraw`/range primitives**. The `predict_mock` module is a pragmatic stand-in *only because the official Predict on-chain indexer/oracle was not yet live during the hackathon* — its interface is already aligned and switching to real Predict is the first post-hackathon step. **Everything that is LadderVault's own — the Move contracts, the testnet deployment, the on-chain transactions — is real.**

**(中文摘要)** 被动 LP 在"价格黏住热门行权价、库存集中中标"时被尾部赔付击穿;LadderVault 用集中度信号自动撤出/回场,链下杀手验证显示削尾 82%(逼近先知上界,可一键复现)。合约已部署 testnet、有真实端到端链上交易、2 个 Move 测试全过。Sui 集成:Move 共享对象金库 + LV 份额 token + PTB 组合的存取/再平衡,接口对齐 DeepBook Predict;predict_mock 仅因官方 Predict 链上设施赛期未就绪而作临时替代,接口已对齐、赛后即切。

## Links / 链接

- **GitHub (code + tests + quant)**: https://github.com/LambertAlpha/LadderVault
- **Demo Video**: https://youtu.be/qb7lspMbuXY
- DeepSurge: _(optional, TODO)_

## Team / 团队成员

- @LambertAlpha

## Deployment / 部署信息

- Env: **Sui Testnet**
- Package ID: `0x1f6134b78470a5d6818e956b53140850a2501f122839d80e6d8d60877e3cc52d`
- Vault (Explorer, 含真实交互历史): https://testnet.suivision.xyz/object/0x0906b259c177763e0898fb8135b608938676de047bf153971d60fdf07034341b
- PredictPool: `0xa9a8a407f4f1698e28a6290e0b800a2bbafed8012bf6587f2eafe0fa202ac17d`

## Swag / 周边

- [x] 我希望接收周边 / I'd like to receive swag
