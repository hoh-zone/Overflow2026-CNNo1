# Auto Lead Flow / 自动线索流

## Track / 赛道

- [ ] Agentic Web
- [ ] DeFi & Payments
- [ ] DeepBook
- [x] Walrus

## Description / 项目简介

Auto Lead Flow is a verifiable social-platform lead automation system that helps configurable industry sales agents discover, qualify, reach out to, and continuously follow up with high-intent customers. It automates the workflow that is usually done manually on social platforms: searching posts and comments for buying intent, extracting structured lead profiles, scoring lead quality, and sending personalized outreach through a real Android phone running the Xiaohongshu app via Midscene and ADB. After the first touch, the system can poll for customer replies, recall previous customer context, generate the next follow-up message, and continue the conversion process until the customer is converted, declines, or reaches the follow-up limit. The agent role, industry scenario, communication tone, qualification fields, and follow-up strategy are configurable through playbooks, so the same system can adapt from real-estate sales to other social lead-generation scenarios. PostgreSQL stores business state and conversation transcripts, MemWal provides long-term customer memory across sessions and workers, and Walrus stores verifiable artifacts such as source evidence, scoring reports, outreach decisions, conversation traces, memory updates, and handoff proofs.

Auto Lead Flow 是一个面向社交平台获客场景的可验证线索自动化系统，帮助可配置的行业销售 Agent 自动发现、识别、触达并持续跟进高意向客户。它自动完成原本需要人工执行的社交平台获客流程：从帖子和评论中搜索购买意向，抽取结构化客户画像，评估线索质量，并通过真实 Android 手机上的小红书 App，结合 Midscene 和 ADB 发送个性化私信触达。在首次触达之后，系统还能轮询客户回复，召回历史客户上下文，生成下一轮跟进话术，并持续推进转化，直到客户转化、拒绝或达到跟进上限。系统的 Agent 角色、行业场景、沟通语气、线索字段和跟进策略都可以通过 playbook 配置，因此不仅适用于房产销售，也可以扩展到其他社交平台获客场景。PostgreSQL 负责保存业务状态和原始对话记录，MemWal 提供跨 session、跨 worker 的长期客户记忆，Walrus 则保存来源证据、评分报告、触达决策、对话 trace、记忆更新和 handoff proof 等可验证 artifacts。

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/545cc3e6-2264-4be1-8a3f-1eb206d88b0a
- GitHub: https://github.com/jethrozz/LeadFlow-Memory
- Demo Video: https://youtu.be/n4Wwd7O1s-c
- Website: TBD

## Team / 团队成员

- @jethrozz

## Deployment / 部署信息

- Env: Testnet
- Package ID: N/A - Walrus artifacts are stored via Walrus testnet publisher/aggregator

## Swag / 周边

- [x] 我希望接收周边 / I'd like to receive swag