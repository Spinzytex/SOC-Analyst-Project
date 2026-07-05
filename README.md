# SOC Triage Range

A single-file, self-contained SOC Tier 1 triage simulator. Every case run
(domains, IPs, usernames, timestamps, ~950 log rows) is procedurally
generated in-browser — nothing is hardcoded, so it can be replayed
indefinitely without repeating.

## Run it
Just open `index.html` in a browser, or visit the GitHub Pages URL once
this repo has Pages enabled.

## Structure
- `index.html` — the entire app (HTML/CSS/JS, no build step, no backend)

## Adding new incident types
See the `SCENARIOS` array and `buildTabs()` / `buildQuestions()` functions
in `index.html`. Each scenario needs a case generator, a set of evidence
tab renderers, and a set of free-text graded questions.
