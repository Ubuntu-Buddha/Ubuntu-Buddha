### Trig Bundgaard

Software engineer shipping AI-native products from the model to the chain: eval-gated LLM features, multi-agent pipelines that stop for a person, and the platforms and on-chain programs underneath. Former Lead Software Engineer (CTO) at Remarc. Colorado Springs, CO · remote US.

[trigbundgaard.com](https://trigbundgaard.com) · [LinkedIn](https://www.linkedin.com/in/trig-bundgaard) · [X](https://x.com/trigbundgaard)

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white)
![Solana](https://img.shields.io/badge/Solana%20%2F%20Anchor-9945FF?style=flat&logo=solana&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

---

## 🛡️ StrangerDanger

An agent that can run commands, and that also reads a web page, an email, or a stranger's repo, can be given its orders by whoever wrote that text. Prompt-injection filters try to catch the bad text, and they miss some. [StrangerDanger](https://github.com/Ubuntu-Buddha/claude-code-stranger-danger) takes the other route: the agent with the shell never reads the untrusted text itself.

- **Readers:** a web page goes to `web-researcher`, which can only search and fetch. A document or a stranger's tree goes to `document-reader` or `quarantine-reviewer`, which can only read files. None of them can run a command or write. What comes back is a report, and the report stays data.
- **Gates:** acting agents are kept off the web, off the folders you mark untrusted, and off secret paths (`~/.ssh`, `.env`, key stores, wallet files). The launch gate refuses the common fetch-and-run forms (`npx`, `uvx`, a download piped into a shell) and `sudo`. Setup turns Claude Code's sandbox on. That sandbox is what contains a shell if a hijack gets through.
- **In your hands:** `/stranger-danger:setup` shows each settings change as a diff and writes nothing until you approve it. Restart, then `/stranger-danger:doctor` checks that the gates are actually loaded in the session you have open.
- **The limit, said plainly:** every agent still runs as you. It can reach your files, keys, and servers through any shell it drives. The hooks constrain tool calls. They do not take that authority away. **v0.2.0, experimental.** MIT.

```
/plugin marketplace add Ubuntu-Buddha/claude-code-stranger-danger#v0.2.0
/plugin install stranger-danger@claude-code-stranger-danger
```

## 🎵 TasteMaker — [tastemaker.music](https://tastemaker.music)

A social platform and a funding layer on Solana: artists post, build a community, and raise against milestones. Designed and built solo, end to end.

- **Platform:** Next.js and React on PostgreSQL (Supabase), Docker behind nginx, GitHub Actions for CI. Vitest on the web app. The web platform is private.
- **AI:** an in-app assistant that works as a platform consultant, hardened against prompt injection, and held to an eval gate before a release. Outreach is a multi-agent pipeline, Scout → Research → Write → QA → Send → Track, with a human review queue, quality gates, and rate limits.
- **On-chain:** [Anchor programs](https://github.com/Tastemaker-inc/tastemaker-programs) on devnet for project escrow, quadratic governance, RWA tokens, revenue distribution, an OTC market, the platform token, and Token-2022 transfer hooks. Milestone funds release through a governance CPI.
- **Media:** FFmpeg transcoding, signed streaming URLs, vector embeddings, a social feed, and messaging.

Code: [Tastemaker-inc/tastemaker-programs](https://github.com/Tastemaker-inc/tastemaker-programs) (public) · web platform private

## 🐂 KEKBULL / ICHOR DAO — [dao.kekbull.com](https://dao.kekbull.com)

An on-chain DAO on Solana mainnet: a holder UI, the ICHOR conversion program, and an SPL Governance fork that fixes voting for Token-2022 mints with transfer fees.

- [`kekbull-governance`](https://github.com/KEKBULL-ICHOR-DAO/kekbull-governance) — SPL Governance 3.1.2 fork with a CastVote / FinalizeVote fix for `TransferFeeConfig` mints · mainnet `2uNHeSLiNn6dLLtiGrpCd8UZKBfV36kap57eg9kV39Fj`
- [`ichor`](https://github.com/KEKBULL-ICHOR-DAO/ichor) — ICHOR conversion program and the client used to verify it · mainnet `DmnfCzQNbx4ZAWEwBoAKqTALgwuUXwYxZL1dRqXoZ1Md`
- [`dao`](https://github.com/KEKBULL-ICHOR-DAO/dao) — holder SPA, Wallet Standard only, no keys in the repo; signing fails closed off its own domain
- [`website`](https://github.com/KEKBULL-ICHOR-DAO/website) — source for [kekbull.com](https://kekbull.com)

## 🤖 Agentic job-search system (private)

A multi-agent pipeline in Python on Claude Code and the Cursor SDK: discovery → knockout rules → LLM tailoring → a verifier that checks every claim against a truth ledger → a separate reviewer model that grades the draft against the posting → browser fill-and-stop over MCP and Playwright. Agents never click Submit. Postings and emails are treated as untrusted input. SQLite state machine with an audit log.

## Earlier

- **Remarc — Lead Software Engineer (CTO), 2020–2025:** the company's loan origination system (a 13-stage pipeline, Dwolla ACH, e-signatures with SHA-256 document integrity) and a customer-facing AI loan advisor on the OpenAI API. Public, sanitized: [`loan-origination-system`](https://github.com/Ubuntu-Buddha/loan-origination-system), [`ai-financial-calculator`](https://github.com/Ubuntu-Buddha/ai-financial-calculator), [`executive-erp-dashboard`](https://github.com/Ubuntu-Buddha/executive-erp-dashboard)
- **Solana libraries:** [`solana-tx-sender`](https://github.com/Ubuntu-Buddha/solana-tx-sender), [`solana-realtime-data`](https://github.com/Ubuntu-Buddha/solana-realtime-data), [`solana-onchain-utils`](https://github.com/Ubuntu-Buddha/solana-onchain-utils), [`alpaca-market-data-pipeline`](https://github.com/Ubuntu-Buddha/alpaca-market-data-pipeline)
- **Ethereum:** [`HYPNOSecosystem`](https://github.com/Ubuntu-Buddha/HYPNOSecosystem) — dual-token DAO governance in Solidity (quadratic voting, an upgradeable proxy). The HYPNOS token is on mainnet.

---

Open to **forward deployed / applied AI**, **AI platform**, and **Solana / blockchain** engineering roles, remote US.
