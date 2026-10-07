# FB Ads Book hosting

The original seven Markdown chapters are published at **https://fbads.toli.me/**. Edit the existing chapters and `SUMMARY.md`; `website/` builds the chapter reader without changing the book's text.

Netlify project `toli-fbadsbook` (`2dbcfacf-578c-4ede-9999-7b5d6cc593f5`) builds the public `tolicodes/fbadsbook` repository on pushes to `master`. Root `netlify.toml` selects base `website`, command `npm run build`, and output `dist`. Netlify manages the `fbads.toli.me` DNS record and HTTPS certificate.

## Local checks

```sh
cd website
npm ci
npm run build
```

October 3, 2026: implementation `477284a` produced seven chapter pages, with all local navigation and assets verified. Netlify deployment `6ac190b66f727b513880c73f` published that commit; all live chapter pages and CSS matched the tested build byte for byte. HTTPS was verified with certificate validation enabled. Public DNS resolvers resolved the new hostname; a local negative DNS cache briefly persisted after creation. The browser loaded the custom domain successfully.

This is the preserved historical guide, not an update to present-day advertising practices. Existing external references remain as authored. Build tooling's `http-cache-semantics` dependency has an advisory with no newer package available during setup; deployed output contains only HTML and CSS, with no server or runtime dependencies.

Toli clarified that the requested portfolio link belongs on **tolicodes.com**, the public Sites portfolio. Its source commit `fdd334d440d6642a8167ff923d3fddba1622f677` changes the FB Ads Book title/action destinations to `https://fbads.toli.me/` and labels the action “Read the book.” The separate `toli.me` source change was reverted in `d64dd07` after this clarification; no Carrd edit is required.

## Public session replay — October 7, 2026

PostHog project 651591 (US), pinned posthog-js 1.438.2, loads asynchronously only on the production canonical hostname. Each session is labeled with `site`. Localhost, preview hosts, Do Not Track and Global Privacy Control skip initialization. Publishable client token is source configuration; no personal API credential is included.

Inputs are masked; private-marked elements are blocked; console logs and network headers/bodies are excluded. Analytics URL properties remove queries, credentials and unknown fragments; this is not a guarantee of redaction of every replay snapshot URL. Public book/page text and images remain visible. No user identification or person profiles are created. Analytics failure does not interrupt rendering.

The production build and all four analytics privacy-policy checks passed before committing. Deployment and receipt of a real recording are verified separately after publication. Existing content, hosting and redirects are preserved.
