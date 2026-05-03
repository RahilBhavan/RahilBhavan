# GitHub account checklist (manual steps on github.com)

Complete these in the GitHub UI so your **profile page** matches the recruiter-optimized [README.md](README.md). Nothing here auto-applies; use this as a launch checklist.

## Profile photo

- [ ] Use a clear, well-lit headshot (or professional-adjacent avatar). Avoid tiny or low-contrast images.

## Bio (≈160 characters)

Copy-paste starting point (trim to fit):

```text
UMich MechE · DeFi risk & on-chain systems · protocol tooling, simulation, TypeScript/Solidity/Rust
```

Adjust keywords to match your **top 1–2 role targets** (e.g. add "smart contracts" or "quant dev").

## Profile URL / social

- [ ] **Settings → Public profile → Website** (or bio field): primary CTA — LinkedIn, portfolio, or calendar link.

## Private contributions (if most code is in private repos)

- [ ] **Settings → Profile → Contributions & activity** → enable **"Include private contributions on my profile"** so the graph shows activity without exposing code ([GitHub Docs](https://docs.github.com/en/account-and-profile/setting-up-and-managing-your-github-profile/customizing-your-profile/using-your-github-profile-to-enhance-your-resume)).

## Pinned repositories (6 slots)

Suggested order (mix of **risk**, **tooling**, **product**); replace if a repo is private or you prefer another public repo.

1. `Smart-Contract-Invariant-Monitor-and-Guardian-` — exploit replay / invariants (strong signal).
2. `summer-fi-risk-analysis` — stress case + methodology write-up.
3. `quant-matrix-v2` — builder + backtest + Web3.
4. `defi-builder` — larger application surface (AI, optimization).
5. `liquidityvector` — execution / yield framing + architecture.
6. `beefy-yield-fidelity-monitor` — dashboard / break-even narrative (README upgraded in-repo).

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
| Smart-Contract-Invariant-Monitor-and-Guardian- | Strong README; optional screenshot of sample report output. |
| summer-fi-risk-analysis | Strong methodology + run steps. |
| quant-matrix-v2 | Strong; consider **Tests** / **Local dev** near top if missing. |
| defi-builder | Strong; keep **Quick start** immediately after intro. |
| liquidityvector | Strong architecture; ensure **Quick start** is easy to find. |
| beefy-yield-fidelity-monitor | README replaced (no CRA boilerplate); Dependabot added via `.github/dependabot.yml`. |

## Before you send applications

- [ ] Open your profile in an **incognito** window: confirm README renders, links work, no broken images.
- [ ] Click **one** pinned repo as a hiring manager would: README makes sense in < 1 minute.

---

## Audit log (readonly profile review)

- **Removed from profile README:** Glitch visitor counter, trophy widget, GitHub Readme Stats, streak-stats (fewer third-party failures; calmer signal for finance hiring).
- **Messaging:** Headline ties **MechE + UMich** to **DeFi / on-chain / simulation** in one scan line.
- **Reliability:** Featured section uses stable GitHub links only (no hotlinked widget images).
