# QuackBench Kingshot Hub — Policies

A **separate, public, static legal-information project** for the QuackBench Kingshot Hub Discord application and planned subscription services. It is intentionally independent from the appointment and bot codebases.

## Contents

- `TERMS.md` — the Terms of Service source of truth.
- `PRIVACY.md` — the Privacy Policy source of truth.
- `LAUNCH_CHECKLIST.md` — details requiring operator confirmation and legal review before paid public launch.
- `index.html`, `terms/`, `privacy/`, `assets/` — pre-rendered accessible static pages. No build process or secrets required.
- `vercel.json` — route rules for `https://<host>/terms` and `https://<host>/privacy`.

## Intended public URLs

- `https://<public-domain>/terms`
- `https://<public-domain>/privacy`

Use these addresses in Discord Developer Portal → General Information after deploying and verifying the pages. A project-specific `.vercel.app` URL is fine until a `quackbench.uk` legal subdomain is configured.

## Deployment

Vercel: deploy the repository root as a static site with `vercel.json` (no build command required). GitHub Pages: choose **Deploy from a branch → main → /(root)**, or configure a custom domain for simple `/terms/` and `/privacy/` paths. Absolute public URLs should only be supplied to Discord after confirming the deployment works.

The policy dates and wording should be approved by the operator and a UK legal professional before making paid services available. Avoid logging or publishing private customer records in this public repo.