# LP Agent

## Track / 赛道

- [x] Agentic Web
- [ ] DeFi & Payments
- [ ] DeepBook
- [ ] Walrus

## Description / 项目简介

LP Agent 是一个开源的 **agent 模板**——你 fork 下来自己运营的参考实现,而非托管应用——用于一个**自主、链上委托的量化做市操作者**:它预测短期价格的*分布*,并围绕该分布塑形 Cetus DLMM 流动性,在赚取手续费的同时捕捉低买高卖的价差,并把闲置资产路由到 Scallop / Kai 借贷生息——所有这些都运行在一个 Move 权限边界内,该边界让"提走资金"在结构上不可能发生:用户始终保有自托管,agent 能动头寸,却永远碰不到出口。它接入 [LeafSheep](https://app.leafsheep.xyz) 的 `PositionManager` 委托槽,通过链上 `AgentAdded` 事件自动发现工作,并把每次再平衡作为一个原子 PTB(collect → remove → transfer → redeem → add → supply)提交。没有中心化服务:每个部署者拥有自己的风险策略、资金上限、计费设计与训练模型。设计主旨——做市是一个预测问题,σ 比 μ 更重要,所以按预测分布(q10/q50/q90)在各 bin 上加权摆放流动性,而非追逐现价。技术栈:Bun + TypeScript + SQLite(agent)· uv + Python + LightGBM(ML 流水线),约 16K LOC,572 个 bun 测试 + ~100 个 pytest 测试,Apache-2.0。仓库交付的是框架与流水线,而非训练好的模型——模型产物(alpha)由 fork 自行训练。

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/b663060f-3e1a-4e53-aac9-c249f38645e4
- GitHub: https://github.com/RandyPen/lp-agent
- Demo Video: https://x.com/pikapikasui/status/2068330609597177940
- Website: https://app.leafsheep.xyz

## Team / 团队成员

- @RandyPen

## Deployment / 部署信息

<!-- LP Agent 是链下运营的 agent 框架,本身没有独立部署的 Move 合约;
     它通过 LeafSheep (CDPM) 已部署在 Sui 主网的 PositionManager 包运行。 -->

- Env: Mainnet
- Package ID: `0xbb15c25329fbc85b9cc9cc1d37ee2f913696a7c688d0552ca4dc7e3557598541` (LeafSheep / CDPM PositionManager — 本项目通过它运行)

## Swag / 周边

- [x] 我希望接收周边 / I'd like to receive swag
