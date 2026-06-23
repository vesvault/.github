# Security Policy

VESvault builds end-to-end encryption tools, so we take security reports
seriously and value the researchers who help keep VES users safe.

This is the **default policy for every repository in the VESvault organization**
(libVES.c, libVES, VESmail, VESlocker, SNIF, and related projects). A repository
may override it with its own `SECURITY.md`.

## Reporting a vulnerability

**Please report security vulnerabilities privately — not through public issues,
pull requests, or Discussions.**

Two ways to reach us:

- **GitHub (preferred)** — open *"Report a vulnerability"* under the **Security**
  tab of the affected repository (private vulnerability reporting). This keeps
  the report confidential until a fix is ready.
- **Email** — **Dev@VESvault.com**. If you'd like to encrypt your report, let us
  know and we'll share a key.

Please include, as far as you can:

- the affected project, version or commit, and platform;
- a description of the issue and its security impact;
- steps to reproduce, a proof of concept, or relevant logs.

## What to expect

- We aim to **acknowledge** your report within **3 business days**.
- We'll validate the issue, keep you updated on remediation, and coordinate a
  disclosure timeline with you.
- With your consent, we're glad to **credit** you when the fix is published.

Please give us a reasonable opportunity to release a fix before any public
disclosure.

## Scope

In scope: vulnerabilities in the source of VESvault repositories — for example
cryptographic flaws, memory-safety bugs, authentication or authorization issues,
and protocol weaknesses.

Generally out of scope: automated-scanner output with no demonstrated impact,
missing security headers on marketing pages, and social-engineering or physical
attacks. When in doubt, send it — we'd rather hear about it.

## Good-faith research

We will not pursue or support legal action against researchers who act in good
faith: who avoid privacy violations, data destruction, and service degradation,
and who give us a reasonable chance to remediate before disclosing.
