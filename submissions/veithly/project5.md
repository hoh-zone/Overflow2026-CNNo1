# DripDeep / 条件式 DCA 策略

## Track / 赛道

- [ ] Agentic Web
- [ ] DeFi & Payments
- [x] DeepBook
- [ ] Walrus

## Description / 项目简介

DripDeep is the first no-code, conditional DCA tool on Sui. Most DCA apps are rigid — "$X every Y days". Real retail wants conditional rules: "buy on dips," "skip flash crashes," "TWAP out on highs." DripDeep makes those rules a three-dropdown click and turns them into a Sui object that fires DeepBook orders only when the condition is true. Reviewer flow: open `/app`, pick "Buy SUI with USDC" / "Every Friday" / "Only if spot < 7d avg by 5%", slide $50, click **Activate strategy on Sui Testnet**. One PTB mints the Strategy object — a keeper loop calls `try_trigger` every minute against Sui Clock; the Move function returns early if the rule is false, otherwise it fires a DeepBook order.

DripDeep 是 Sui 上第一个面向散户的条件式 DCA 工具。市面上 DCA 都是 "每 X 天买 Y 元"，但真实的零售用户想要"逢跌买入、闪崩跳过、高位 TWAP 卖出"这种条件化规则。DripDeep 把这些规则做成三个下拉框就能配置，并写成 Sui 对象——只有条件满足时才往 DeepBook 下单。评审流程：`/app` → 选 "Buy SUI with USDC" / "Every Friday" / "Only if spot < 7d avg by 5%"，金额 $50，点击 **Activate strategy on Sui Testnet**。一笔 Move 调用交易铸造 Strategy 对象，keeper 每分钟基于 Sui Clock 调用 `try_trigger`，规则不满足直接 early return，满足才下 DeepBook 订单。

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/project/df2f6929-8e00-4c46-a3a8-903431095575
- GitHub: https://github.com/veithly/dripdeep
- Demo Video: https://youtu.be/EFkULL4_Qe4
- Website: https://dripdeep.veithly.workers.dev

## Team / 团队成员

- @veithly

## Deployment / 部署信息

- Env: Testnet
- Package ID: 0x74436e36e7d5c8400eadaa9d10540a6f9c7d328705bf2241211009b5a3b5d5c6

## Swag / 周边

- [x] 我希望接收周边 / I'd like to receive swag
