# AntFleet org house rules — repository naming & layout

Standing rules for keeping the `antfleet` GitHub org tidy. Adopted 2026-07-11.

## 1. Benchmark mirrors

A benchmark mirror is a standalone snapshot of an external project that AntFleet ran
through its two-model unanimous security-review methodology.

- **Name:** `bench-<upstream-repo>`. Prefix only. Never the `<name>-bench` suffix form.
  - Use the upstream *repo* name. Add an org qualifier only to disambiguate collisions
    (e.g. `bench-virtuals-acp-cli` vs a hypothetical other `acp-cli`).
- **Description format:**
  `AntFleet benchmark mirror of <owner>/<repo> — two-model security review methodology`
  Do **not** copy the upstream project's marketing tagline; that hides that it's a mirror.
- **Keep mirrors as separate repos.** Do not collapse into a monorepo — the review is
  only valid against the real, unmodified source, and receipts pin to the upstream URL.
- **Catalog:** every mirror is listed in [`antfleet/bench`](https://github.com/antfleet/bench)
  `README.md`. Add a row when you create a mirror; the master repo is the index of record.
- **Visibility:** public by default; private only when the upstream or engagement requires
  it (e.g. `bench-localai`).

## 2. Not-a-mirror repos with "bench" in the name

Products and templates keep product names and are excluded from the mirror index:
- `open-evmbench` — public leaderboard product.
- `aeon-template` — productized review template (formerly `aeon-bench`).

If a repo isn't a review snapshot, its name must not read as `bench-<something>`.

## 3. Receipts & findings are immutable

Published findings / receipts record history. Never rewrite them to match a rename;
GitHub redirects keep old mirror URLs alive, and receipts point at the upstream repo
anyway. Renaming a mirror is safe and does not touch receipt provenance.

## 4. Renames

Prefer `gh repo rename` (preserves redirects) over delete-and-recreate (kills redirects,
404s external links). All AntFleet org writes go through the `antfleet-ops` account.

---

_Normalization complete 2026-07-11: all 22 mirror descriptions follow the § 1 format and
every upstream is filled in the [index](./README.md)._
