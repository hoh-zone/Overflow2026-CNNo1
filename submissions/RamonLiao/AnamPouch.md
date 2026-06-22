# AnamPouch

## Track / 赛道

<!-- 选择一个赛道，把 [ ] 改成 [x] / Select one track -->

- [ ] Agentic Web
- [ ] DeFi & Payments
- [ ] DeepBook
- [x] Walrus

## Description / 项目简介

<!-- 一段话描述你的项目：做什么，为什么重要 / What it does, why it matters -->

*   **Business Pain Points**: Clinical health data is fragmented across clinics, leaving patients without access. Furthermore, sending audio consultations, certificates, and medication photos to the cloud for AI analysis raises severe HIPAA compliance and data leakage concerns.
    *   **Solution**: AnamPouch provides a privacy-first, patient-sovereign digital medical pouch. A local client-side 3B-8B LLM processes records in-browser, encrypting data with a client-derived AES key before storing it on Walrus. Patients share records with doctors via time-locked, on-chain Seal grants, allowing instant web decrypts under sponsored gas.
    *   **Key Features**:
        1. **zkLogin & Browser Encryption**: Google OAuth sign-in derives non-custodial keys to run in-memory AES-GCM-256 encryption.
        2. **Client-Side AI Processing**: Transcribes audio, OCRs reports, and checks drug interactions locally.
        3. **Walrus Pouch Storage**: Encrypted files reside on Walrus, with records anchored to Sui transaction hashes.
        4. **On-Chain Access Grants**: Move-enforced time-locked grants allow doctors to view data with zero wallet/gas requirements.

## Links / 链接

- DeepSurge: https://www.deepsurge.xyz/projects/a541d658-8110-4fea-b49c-7f557e688788
- GitHub: https://github.com/RamonLiao/AnamPouchV2
- Demo Video: https://... (YouTube, ≤ 5 min)
- Website: https://anam-pouch.vercel.app (optional)

## Team / 团队成员

<!-- 列出所有成员 of GitHub ID / List all team members' GitHub IDs -->

- @RamonLiao

## Deployment / 部署信息

<!-- 填写部署环境和合约地址 / Fill in deployment env and package ID -->

- Env: Testnet
- Package ID: `0x003541284dfd4ff30719150942dda62970c1643d4d5fa7abf6183819c903bbd5`

## Swag / 周边

<!-- 如需接收周边，勾选即可，收件信息请通过表单提交（见 guide.md）/ Check if you want swag, submit shipping info via the form -->

- [ ] 我希望接收周边 / I'd like to receive swag
