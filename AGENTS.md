# BeltBench Devlog contributor guide

## Scope and language

- This is a public engineering-record site.
- Keep the narrative structure of every visitor-facing web page, issue title,
  body text, caption, and news item in Korean. Retain established technical
  terms in English when translating them would be awkward or less precise
  (for example: Modular, VLA, trial, runtime, adapter, and hand-eye
  calibration).
- Keep repository-management documents, instructions, metadata, commit
  messages, and other non-site files in English.
- The private BeltBench repository owns implementation code. This repository
  records decisions and sanitized evidence; it does not mirror code trees.

## Media and security

- Photos, screenshots, short videos, and diagrams are welcome when they make
  an issue easier to understand.
- Strip EXIF location data before publishing. Inspect media for device
  identifiers, IP/MAC addresses, hostnames, internal paths, accounts, tokens,
  private calibration, and raw datasets.
- If sensitive material is published, remove the asset and references
  immediately, then rewrite the public Git history as appropriate.

## Issue-page contract

Each issue page should cover:

1. problem and impact;
2. observed evidence, with sanitized media where useful;
3. diagnosis;
4. resolution procedure or current blocker;
5. verification;
6. related issues and next action.

Every implementation or investigation session must leave a chronological record
that separates facts from hypotheses. Include the exact source revision and
environment identity when they affect reproducibility. Record failed attempts:
the symptom, direct evidence, root cause or current hypothesis, corrective
action, and verification result are part of the research output.

Use these status labels consistently:

- `planned`: contract and acceptance evidence are defined, implementation absent;
- `in progress`: implementation or verification is incomplete;
- `blocked`: the unmet external condition and safe next action are explicit;
- `verified`: the stated acceptance evidence passed at a recorded revision.

Do not use `verified` for a structural smoke test when algorithmic accuracy was
not measured. State the verification boundary directly.

## Maintenance rules

- Put new issue pages under issues/<area>/ and link them from issues/index.html
  and the homepage news section.
- Keep approved assets under assets/images/ using descriptive filenames.
- Validate the local site before pushing to the public remote.
- Add each new issue to `issues/index.html`; add only current, high-value work to
  the homepage. Check links and serve the site locally before publishing.
- Update an existing issue rather than creating a success-only duplicate. Append
  dated verification notes so that regressions and superseded conclusions remain
  traceable.
