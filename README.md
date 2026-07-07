# Auto quickstart

A ready-to-roll software factory running on [Auto](https://auto.sh). This repo ships a complete agent fleet in [`.auto/`](.auto) — onboarding, PR review, handoff, and self-improvement — plus a small site in [`site/`](site) that the fleet builds, reviews, and republishes on every merge to `main`.

To get started, click **Use this template** above to create your own copy (forking works too), then connect GitHub in Auto setup and pick your new repo. Auto detects the `.auto/` configuration on the default branch, syncs the whole fleet automatically — no bootstrap PR — and opens an onboarding session that walks you through the rest.

From there the loop runs itself: every merge redeploys `site/` to [here.now](https://here.now) and posts the live URL as a commit comment, the PR reviewer covers every pull request, and once the onboarding agent wires the site's request bar, anyone with the passphrase can ask for a change right on the page and a coding agent will pick it up.
