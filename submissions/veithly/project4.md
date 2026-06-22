# TrustClip / 视频证据上链

## Track / 赛道

- [ ] Agentic Web
- [ ] DeFi & Payments
- [ ] DeepBook
- [x] Walrus

## Description / 项目简介

TrustClip turns any video into a tamper-evident artifact in 5 seconds. Drop a clip into the page, the bytes chunk directly to Walrus, the SHA-256 is computed in your browser, and one PTB mints a Sui `Witness` object with the blob_id + sha256 + timestamp. Share `/w/[id]` with anyone — they play the original from Walrus and verify the on-chain Witness without an account or wallet install. Reviewer flow: open `/app`, pick a sample clip (dashcam fender-bender, citizen-journalist street scene, building inspector visit), click **Mint witness on Sui Testnet** — the trial wallet signs a real Sui PTB and pins the witness on-chain in front of you.

TrustClip 让任何视频在 5 秒内成为防篡改证据。把视频拖入页面，浏览器端分块上传到 Walrus、本地计算 SHA-256，一笔 Move 调用交易在 Sui 上铸造 `Witness` 对象（blob_id + sha256 + timestamp）。分享 `/w/[id]` 给任何人——他们直接从 Walrus 拉源文件、对照链上 Witness 校验，不需要钱包不需要注册。评审流程：`/app` 选一个样本视频（行车记录碰撞 / 公民新闻 / 建筑验房），点击 **Mint witness on Sui Testnet**，trial wallet 现场签发真实 Sui Move 调用，digest 可在 suivision.xyz 验证。

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/project/33a9ed98-a81c-471d-86b6-9bfff676b5c6
- GitHub: https://github.com/veithly/trustclip
- Demo Video: https://youtu.be/6s9wotEz5mk
- Website: https://trustclip.veithly.workers.dev

## Team / 团队成员

- @veithly

## Deployment / 部署信息

- Env: Testnet
- Package ID: 0x4f36930c8b4ece4e18cdedc7cd8c9b90d3aacea64b9a19c49502ca60ee7d6bc0

## Swag / 周边

- [x] 我希望接收周边 / I'd like to receive swag
