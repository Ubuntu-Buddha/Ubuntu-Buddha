### Trig Bundgaard

Software engineer who ships AI-native products end to end: LLM features with eval gates, multi-agent pipelines with a human in the loop, and the platforms and on-chain programs under them. Former Lead Software Engineer (CTO) at Remarc. Colorado Springs, CO · remote US.

[trigbundgaard.com](https://trigbundgaard.com) · [LinkedIn](https://www.linkedin.com/in/trig-bundgaard) · [X](https://x.com/trigbundgaard)

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white)
![Solana](https://img.shields.io/badge/Solana%20%2F%20Anchor-9945FF?style=flat&logo=solana&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

---

## 🎵 TasteMaker — [tastemaker.music](https://tastemaker.music)

A social platform and funding layer on Solana: artists post, build communities, and raise with milestones. Designed and built solo, end to end.

- **Platform:** Next.js 15 / React 19 / PostgreSQL (Supabase) — 127 API routes, 49 pages, 105 database migrations, Vitest suite; Docker deploy behind nginx, GitHub Actions CI
- **AI:** an in-app assistant that works as a platform consultant, released only on a **≥98% eval pass rate** and hardened against prompt injection; a multi-agent outreach pipeline (Scout → Research → Write → QA → Send → Track) with a human-in-the-loop review queue, quality gates and rate limits
- **On-chain:** [7 Anchor programs](https://github.com/Tastemaker-inc/tastemaker-programs) on devnet — project escrow, quadratic governance, RWA tokens, revenue distribution, OTC market, platform token, Token-2022 transfer hooks. Milestone funds release only through a governance CPI, with no admin bypass; 77 integration tests simulate a 40-backer, 5-milestone lifecycle
- **Media:** FFmpeg transcoding, signed streaming URLs, vector embeddings, social feed and messaging

Code: [Tastemaker-inc/tastemaker-programs](https://github.com/Tastemaker-inc/tastemaker-programs) (public) · web platform private

## 🐂 KEKBULL / ICHOR DAO — [dao.kekbull.com](https://dao.kekbull.com)

On-chain DAO on Solana **mainnet**: a holder UI, the ICHOR conversion program, and an SPL Governance fork that fixes voting for Token-2022 mints with transfer fees.

- [`kekbull-governance`](https://github.com/KEKBULL-ICHOR-DAO/kekbull-governance) — SPL Governance 3.1.2 fork with a CastVote / FinalizeVote fix for `TransferFeeConfig` mints · mainnet `2uNHeSLiNn6dLLtiGrpCd8UZKBfV36kap57eg9kV39Fj`
- [`ichor`](https://github.com/KEKBULL-ICHOR-DAO/ichor) — ICHOR conversion program and the client used to verify it · mainnet `DmnfCzQNbx4ZAWEwBoAKqTALgwuUXwYxZL1dRqXoZ1Md`
- [`dao`](https://github.com/KEKBULL-ICHOR-DAO/dao) — holder SPA, Wallet Standard only, no keys in the repo; signing fails closed off its own domain
- [`website`](https://github.com/KEKBULL-ICHOR-DAO/website) — source for [kekbull.com](https://kekbull.com)

## 🤖 Agentic job-search system (private)

A multi-agent pipeline in Python on Claude Code and the Cursor SDK: discovery → knockout rules → LLM tailoring → a verifier that checks every claim against a truth ledger → a separate reviewer model that grades the draft against the posting → browser fill-and-stop over MCP and Playwright. Agents never click Submit. Postings and emails are treated as untrusted input. SQLite state machine with an audit log; 1,280+ tests.

## Earlier

- **Remarc Vending — Lead Software Engineer (CTO), 2020–2025:** led a 5-person team through 400% revenue growth ($900K → $4.4M); built the loan origination system (13-stage pipeline, Dwolla ACH, e-signatures with SHA-256 document integrity) and a customer-facing AI loan advisor on the OpenAI API. Public, sanitized: [`loan-origination-system`](https://github.com/Ubuntu-Buddha/loan-origination-system), [`ai-financial-calculator`](https://github.com/Ubuntu-Buddha/ai-financial-calculator), [`executive-erp-dashboard`](https://github.com/Ubuntu-Buddha/executive-erp-dashboard)
- **Solana libraries:** [`solana-tx-sender`](https://github.com/Ubuntu-Buddha/solana-tx-sender), [`solana-realtime-data`](https://github.com/Ubuntu-Buddha/solana-realtime-data), [`solana-onchain-utils`](https://github.com/Ubuntu-Buddha/solana-onchain-utils), [`alpaca-market-data-pipeline`](https://github.com/Ubuntu-Buddha/alpaca-market-data-pipeline)
- **Ethereum:** [`HYPNOSecosystem`](https://github.com/Ubuntu-Buddha/HYPNOSecosystem) — dual-token DAO governance in Solidity (quadratic voting, upgradeable proxy), deployed to mainnet

---

Open to **forward deployed / applied AI**, **AI platform**, and **Solana / blockchain** engineering roles, remote US.
