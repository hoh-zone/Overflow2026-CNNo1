# Tidecast

## Track / 赛道

- [ ] Agentic Web
- [ ] DeFi & Payments
- [x] DeepBook
- [ ] Walrus

## Description / 项目简介

Tidecast is the desktop trading desk for **DeepBook Predict**, Sui's on-chain BTC prediction market priced by a live SVI volatility surface. Most front-ends on Predict are web or Telegram apps that wrap it as a bet button, a chat assistant, or a payoff-curve builder — Tidecast is built for whoever actually prices the trade. It draws the live SVI vol smile and a per-strike positioning heatmap (strike × implied volatility), prices every strike with gas-free `devInspect` quotes, and mints or redeems in one click: a PTB signed in-process by a local Ed25519 keypair — no wallet extension, no popup. Pure integration, no Move package of its own; the on-chain logic *is* DeepBook Predict. Verified on testnet — real mint digest `8wDTPzWhoq9YKVT95nVKJnBjqmMkPF1UNKCxvgiZmUif`.

Tidecast 是 **DeepBook Predict**（Sui 链上 BTC 预测市场，由实时 SVI 波动率曲面定价）的桌面交易终端。同协议上的其他前端多是网页/Telegram 的下注按钮、聊天助手或收益曲线工具；Tidecast 是给真正定价的人用的交易台：画出实时 SVI 波动率微笑曲线 + 逐 strike 持仓热力图（strike × 隐含波动率），用 `devInspect` 免 gas 实时报价，一键链上 mint/redeem（本地 Ed25519 密钥进程内签名，无钱包插件、无弹窗）。纯集成、无自有 Move 包，链上逻辑即 DeepBook Predict。testnet 真实集成，mint digest：`8wDTPzWhoq9YKVT95nVKJnBjqmMkPF1UNKCxvgiZmUif`。

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/b97130ea-2af1-497e-a8d5-ab119350e8dc
- GitHub: https://github.com/JinHe9527/tidecast
- Demo Video: https://drive.google.com/file/d/1by7WOlY4-PWlzGqEdnCeQTP4UcasZqN5/view
- Website: https://tidecast-7q7.pages.dev

## Team / 团队成员

- JinHe9527 (@JinHe9527) — solo

## Deployment / 部署信息

- Env: Testnet
- Package ID: integrates DeepBook Predict `0xf5ea2b3749c65d6e56507cc35388719aadb28f9cab873696a2f8687f5c785138` (pure integration, no own package)
- Our PredictManager (shared object): `0xbee649118662e9081042de04bb4796d224768ae8d5ef51e39c8daa7e0d575bd1`
- Proof — real testnet mint: `8wDTPzWhoq9YKVT95nVKJnBjqmMkPF1UNKCxvgiZmUif`

## Swag / 周边

- [ ] 我希望接收周边 / I'd like to receive swag
