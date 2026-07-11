# antfleet/bench — benchmark mirror index

The single home for AntFleet's public benchmark mirrors. Each `bench-*` repo is a
**standalone, faithful snapshot** of an external project that AntFleet ran through
its two-model unanimous security-review methodology. They live as separate repos on
purpose — the review is only credible if it runs against the real, unmodified source
at a pinned commit. This repo is the catalog, not a monorepo.

> Public receipts pin to the **upstream** repo (e.g. `github.com/mudler/LocalAI/blob/<sha>/...`),
> not to the mirror. The mirror is AntFleet's immutable copy of exactly what was reviewed,
> in case upstream force-pushes or disappears.

## Naming convention (house rule)

- Every benchmark mirror is named **`bench-<upstream-repo>`**. Prefix, never suffix.
- The prefix makes all mirrors sort as one contiguous block in the org repo list.
- Non-mirror bench products keep product names and are **not** in this index
  (e.g. `open-evmbench` = public leaderboard; `aeon-template` = productized template).
- Repo description format: `AntFleet benchmark mirror of <owner>/<repo> — two-model security review methodology`.

See [HOUSE-RULES.md](./HOUSE-RULES.md) for the full org tidy-up rules.

## Mirrors (22)

| Mirror | Upstream | Visibility |
|---|---|---|
| [bench-agent-autonomopoly](https://github.com/antfleet/bench-agent-autonomopoly) | Liquid-Protocol-Ops/agent-autonomopoly | public |
| [bench-agent-openhuman](https://github.com/antfleet/bench-agent-openhuman) | tinyhumansai/openhuman | public |
| [bench-agentfloat](https://github.com/antfleet/bench-agentfloat) | ronkenx9/agentfloat-hook | public |
| [bench-antseed](https://github.com/antfleet/bench-antseed) | AntSeed/antseed | public |
| [bench-bankrskills](https://github.com/antfleet/bench-bankrskills) | BankrBot/skills | public |
| [bench-berry](https://github.com/antfleet/bench-berry) | levyonchain/Berry-Juicer-Public | public |
| [bench-bitterbot-desktop](https://github.com/antfleet/bench-bitterbot-desktop) | Bitterbot-AI/bitterbot-desktop | public |
| [bench-claude-mem](https://github.com/antfleet/bench-claude-mem) | thedotmack/claude-mem | public |
| [bench-doppler](https://github.com/antfleet/bench-doppler) | whetstoneresearch/doppler | public |
| [bench-hermes-desktop](https://github.com/antfleet/bench-hermes-desktop) | fathah/hermes-desktop | public |
| [bench-localai](https://github.com/antfleet/bench-localai) | mudler/LocalAI | private |
| [bench-miroshark](https://github.com/antfleet/bench-miroshark) | aaronjmars/MiroShark | public |
| [bench-mythos-router](https://github.com/antfleet/bench-mythos-router) | thewaltero/mythos-router | public |
| [bench-openclaude](https://github.com/antfleet/bench-openclaude) | Gitlawb/openclaude | public |
| [bench-orlixai](https://github.com/antfleet/bench-orlixai) | tylerbroqs/orlixai | public |
| [bench-reppo-cli](https://github.com/antfleet/bench-reppo-cli) | Reppo-Labs/reppo-cli | public |
| [bench-reppo-polyagent](https://github.com/antfleet/bench-reppo-polyagent) | Reppo-Labs/reppo-polyagent | public |
| [bench-roboco](https://github.com/antfleet/bench-roboco) | rennf93/roboco | public |
| [bench-shh](https://github.com/antfleet/bench-shh) | privashh/shh | public |
| [bench-synthethic](https://github.com/antfleet/bench-synthethic) | AISynthetics/synthetic-users | public |
| [bench-virtuals-acp-cli](https://github.com/antfleet/bench-virtuals-acp-cli) | Virtual-Protocol/acp-cli | public |
| [bench-virtuals-acp-node-v2](https://github.com/antfleet/bench-virtuals-acp-node-v2) | Virtual-Protocol/acp-node-v2 | public |

All 22 mirror descriptions follow the § 1 format `AntFleet benchmark mirror of <owner>/<repo>`.

## Not in this index (bench-named but not mirrors)

| Repo | What it actually is |
|---|---|
| `open-evmbench` | Public leaderboard for AI smart-contract vulnerability work — a product, not a mirror. |
| `aeon-template` | Productized two-model-consensus review template (was `aeon-bench`). Renamed to stop it reading as a mirror. |
