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

## Maintenance rules

- Put new issue pages under issues/<area>/ and link them from issues/index.html
  and the homepage news section.
- Keep approved assets under assets/images/ using descriptive filenames.
- Validate the local site before pushing to the public remote.
