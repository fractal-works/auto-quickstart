# Auto quickstart

A ready-to-roll software factory running on [Auto](https://auto.sh). This repo ships a complete agent starter-pack in [`.auto/`](.auto), with an onboarding agent, a PR review agent, a handoff agent, and a self-improvement agent. It also includes a small site in [`site/`](site) that the agents build, review, and republish on every merge to `main`.

To get started, click **Use this template** above to create your own copy (forking works too), then connect GitHub in Auto setup and pick your new repo. Auto detects the `.auto/` configuration on the default branch, syncs the whole fleet automatically, and opens an onboarding session that walks you through the rest.

From there the loop runs itself: every merge redeploys `site/` to [here.now](https://here.now) and posts the live URL as a commit comment. Once the onboarding agent wires the site's request bar, anyone with the passphrase can ask for a change right on the page and a coding agent will pick it up.
