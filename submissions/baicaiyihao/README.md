# SUI Intent Engine

> **Speak the trade. Chain obeys.**
> Natural language → Guardian risk check → human-readable PTB preview → wallet-signed DeepBook V3 execution on Sui mainnet.

## Track

- [x] Agentic Web
  - **Sub-track 3: Intent Engine**

> Sub-track 3 requires: `text → PTB → execution` + human-readable PTB preview + Guardian with ≥ 2 risk dimensions + explicit user confirmation. This project ships a **6-dimension Guardian** (RSI · MACD · Bollinger · KDJ · Volume · ADX) — well past the bar.

## What it does

Say *"buy 1 SUI if RSI < 30, 2% slippage"* in plain English. The engine runs a 4-step loop:

1. **PARSE** — LLM compiles the sentence into a structured intent (action, size, price, triggers)
2. **GUARD** — Guardian runs the 6-dim risk check and surfaces slippage, weak trend, low liquidity, reversal risk in plain language
3. **PREVIEW** — human-readable PTB card: price, size, total cost, expiry, balance check. No black box.
4. **SIGN** — you confirm, your wallet signs, **DeepBook V3 executes on Sui mainnet**

Why this is Sub-track 3 (not a chatbot):
- Guardian is product differentiation, not LLM wrapper
- Wallet signature + explicit confirm = user is always in the loop
- Real on-chain execution (not simulated), with full BalanceManager lifecycle

## Quick Start

The whole stack boots with **one command**:

```bash
git clone https://github.com/baicaiyihao/sui-intent-engine.git
cd sui-intent-engine
./start.sh           # auto-installs deps, starts :3000 / :8000 / :8001
# → http://localhost:3000
```

`./start.sh` auto-detects `conda:crawl4ai` → `.venv` → creates `.venv`, runs `npm install` on first boot. PIDs in `.pids/`, logs in `logs/`. Shut down with `./stop.sh`. Full README in the repo.

## Links

- GitHub: https://github.com/baicaiyihao/sui-intent-engine
- Landing page: https://github.com/baicaiyihao/sui-intent-engine#readme
- Demo video: to be added via a follow-up PR before deadline

## Team

- @baicaiyihao

## Deployment

- **Network:** Sui mainnet
- **Own Move contract** `sui_intent_fee::protocol_fee` (11/11 unit tests pass) — 0.005 SUI protocol fee per intent, paid to a shared `ProtocolTreasury` object

### Own contract

| Name | ID | Purpose |
|---|---|---|
| `sui_intent_fee` package | `0xad95919bbc8e08a36c28bf885fd7e8413296f63979d13b329d8713424157fd90` | Move 2024.beta protocol-fee module |
| `ProtocolTreasury` (shared) | `0x5e54f169aa2df2c3fe2a7624170d1c85feb7ebf9b54f57e51cb80fc84578ed91` | Receives 0.005 SUI per intent |
| `UpgradeCap` | `0x78386b44de6fb0d19cefa3722ceb3f1ef85da3456ded7fd19ad2e7e1bd7773cf` | Contract upgrade authority |
| Admin (deployer) | `0x90abb670800b4015229d30f5d010faef0c347e1d9650c9acebe2c012be7eb724` | Contract admin |

- End-to-end mainnet tx (pays the fee): `4jGNB1W56Ehfy73nHEyfrK48XxQmWkzcDePVPxehvG1D`
- Testnet package: `0x9e7d5e8048f44773afede881ebb65422c01f686cfe2f141fb7bf9ef002859465`
- Default fee: 0.005 SUI / intent (5,000,000 MIST)
- Events: `FeePaid` / `FeeWithdrawn` / `FeeUpdated` / `AdminTransferred` (chain-indexable for dashboards)

### External Sui contracts used

| Contract | Package ID | Purpose |
|---|---|---|
| DeepBook V1 Pool | `0x2c8d603bc51326b8c13cef9dd07031a408a48dddb541963357661df5d3204809` | Limit / market orders, withdraw, claim |
| Cetus DeepBook Utils | `0x600138d3179e2fc746f6774f360a6e1fa68e90d66d082af66399adabe46f22a4` | One-PTB deposit + place order |
| DeepBook V3 Global Config | `0xff1141ef80e7baf206c7930c274b465600e64884d8167f90d4cdb60197925163` | Cetus utils entry point |
| SUI/USDC Pool | `0xe05dafb5133bcffb8d59f4e12465dc0e9faeaa05e3e342a08fe135800e3e4407` | Live trading pool |

Test wallet (dev only — production users use their own): `0xc52aa1eb1eca93287966af0f12d5fce3b959d3ae598673b90e539987916bc64e`. Full tx history in the repo's `AGENTS.md`.

## Swag

- [x] I'd like to receive swag
  > Mainland China shipping address. Recipient info will be submitted separately via the swag form, not exposed in the public PR.
