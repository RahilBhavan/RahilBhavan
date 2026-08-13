# GitHub account checklist (manual steps on github.com)

Complete these in the GitHub UI so your **profile page** matches the recruiter-optimized [README.md](README.md). Nothing here auto-applies; use this as a launch checklist.

## Profile photo

- [ ] Use a clear, well-lit headshot (or professional-adjacent avatar). Avoid tiny or low-contrast images.

## Bio (≈160 characters)

Copy-paste starting point (trim to fit):

```text
UMich CS+Econ · DeFi risk & on-chain systems · protocol tooling, simulation, TypeScript/Solidity/Rust
```

Adjust keywords to match your **top 1–2 role targets** (e.g. add "smart contracts" or "quant dev").

## Profile URL / social

- [ ] **Settings → Public profile → Website** (or bio field): primary CTA — LinkedIn, portfolio, or calendar link.

## Private contributions (if most code is in private repos)

- [ ] **Settings → Profile → Contributions & activity** → enable **"Include private contributions on my profile"** so the graph shows activity without exposing code ([GitHub Docs](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/using-your-github-profile-to-enhance-your-resume)).

## Pinned repositories (6 slots)

Matches the README's **Featured work** table — keep the two in sync going forward; if you retire a repo from one, retire it from both.

1. `summer-fi-risk-analysis` — stress case + methodology write-up.
2. `beefy-yield-fidelity-monitor` — dashboard / break-even narrative (README upgraded in-repo).
3. `KYA` — decentralized underwriting for AI agent identities (ERC-6551, 4337-aware).
4. `gm_mecg` — automotive supply-chain quarterly financials pipeline.
5. `wingbits` — Wingbits Customer API TypeScript SDK + CLI.
6. *(open slot)* — add a 6th public repo if you want one; otherwise leave 5 pinned.

**For each pin:** on the repo → **⚙ About** → short description, **Topics** (e.g. `defi`, `nextjs`, `solidity`, `risk`), **Website** if you have a demo deploy.

## README quality (30-second rule)

For each pinned repo, the root README should answer quickly:

1. **What** is this (one sentence, plain English)?
2. **Why** it exists (problem / user).
3. **How to run** (3–5 commands max) or link to detailed docs.
4. **Demo** — screenshot, GIF, or live URL above the fold when possible.
5. **Status** — active / research / archived.
6. **Tests / CI** — badge or "how to test" section where applicable.

## Pinned repos — maintenance snapshot

| Repository | Notes |
|------------|--------|
| summer-fi-risk-analysis | Strong methodology + run steps. |
| beefy-yield-fidelity-monitor | README replaced (no CRA boilerplate); Dependabot added via `.github/dependabot.yml`. |
| KYA | Confirm README has Quick start + status (active / research / archived). |
| gm_mecg | Confirm README has Quick start + status (active / research / archived). |
| wingbits | Confirm README has Quick start + status (active / research / archived). |

## Before you send applications

- [ ] Open your profile in an **incognito** window: confirm README renders, links work, no broken images.
- [ ] Click **one** pinned repo as a hiring manager would: README makes sense in < 1 minute.

---

## Audit log (readonly profile review)

- **2026-08-13:** Removed the GitHub Readme Stats cards and profile-trophy widget from `README.md` — both were live-broken (503 / 402 from their hosting services) despite this log previously claiming they'd been removed. Kept `streak-stats` (verified working). Fixed the CompE/MechE mismatch between the README headline and this checklist's bio copy. Re-synced the pinned-repo list above to match the README's Featured work table (they'd drifted after outdated projects were removed from the README).
- **Messaging:** Headline ties **UMich Computer Engineering and Economics** to **DeFi / on-chain / simulation** in one scan line.
- **Reliability:** Featured section uses stable GitHub links only (no hotlinked widget images).
