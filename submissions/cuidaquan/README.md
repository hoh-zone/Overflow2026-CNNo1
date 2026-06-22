# NoFlake on Sui / 不鸽-链上RSVP押金结算

## Track / 赛道

<!-- 选择一个赛道，把 [ ] 改成 [x] / Select one track -->

- [ ] Agentic Web
- [x] DeFi & Payments
- [ ] DeepBook
- [ ] Walrus

## Description / 项目简介

NoFlake is a Sui-native programmable RSVP deposit settlement layer for small community events. Free RSVPs are easy to abandon; NoFlake turns RSVP into a refundable on-chain commitment. Attendees reserve a seat with Circle testnet USDC, deposits are held in an event-specific Move vault, check-in immediately refunds attendees, and no-show deposits are settled by transparent Move rules. The current resubmission also includes attendee reservation cancellation, host event cancellation with attendee refund claims, Strict Mode testnet E2E proof, and a robust check-in fallback path: camera scan, JS QR frame decoding, QR screenshot upload, and manual payload paste. The submitted demo shows a complete Sui testnet flow: 3 attendees reserved seats, 2 checked in and received refunds, and 1 no-show deposit was distributed through Party Mode.

NoFlake 是一个基于 Sui 的 RSVP 押金结算项目，用链上稳定币押金解决线下活动 RSVP 容易爽约的问题。参会者使用 Circle testnet USDC 锁定名额，押金进入 Move 合约托管的活动 vault；到场签到时立即退款，未到场押金按公开规则结算。当前重新提交版本还补充了参会者自主取消报名、主办方取消整场活动并由参会者自助领取退款、Strict Mode testnet E2E 证明，以及更稳的签到二维码流程：摄像头扫码、JS 帧解码、上传二维码截图、手工粘贴 payload。本次 demo 已在 Sui testnet 跑通完整流程：3 人报名、2 人签到退款、1 人 no-show，并通过 Party Mode 完成最终结算。

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/3c9d48b4-d0c4-4a4f-904a-4a6e91e7bd23
- GitHub: https://github.com/cuidaquan/noflake-sui
- Demo Video: https://youtu.be/CmTM3TNDl-8
- Website: https://cuidaquan.github.io/noflake-sui/

## Team / 团队成员

<!-- 列出所有成员的 GitHub ID / List all team members' GitHub IDs -->

- @cuidaquan

## Deployment / 部署信息

<!-- 填写部署环境和合约地址 / Fill in deployment env and package ID -->

- Env: Testnet
- Callable Package ID: `0x7d0b8b3e9b655e5dfe28592009a87f67f667fc6619319c89d786251d45150f5c`
- Original Package / Event Namespace: `0xd4936b362763713dd61fe8bb17fb6c80857ab8a96e91f132ab3f57970ebd37ef`
- Demo event ID: `0xa68fa833ceaa8fb6af92d6e91914e4c4849fb138ea1823d1a96dfce85672a056`
- Settlement receipt ID: `0x06c46a4492fa7bf1124bc351cfc8e299a2d4c108e6dd7e331490e024d25e16e1`

## Swag / 周边

<!-- 如需接收周边，勾选即可，收件信息请通过表单提交（见 guide.md）/ Check if you want swag, submit shipping info via the form -->

- [x] 我希望接收周边 / I'd like to receive swag
