# Yumeniwa 夢庭

*A one-stop tracker for otakus: anime, manga, light novels, visual novels and games, in one place you control.*

> **Status:** under development. Design and decisions live in the wiki: [`yumeniwa/docs/yumeniwaDocumentation.pdf`](yumeniwa/docs/yumeniwaDocumentation.pdf).

## Why it exists

Tracking what you watch, read and play is scattered across apps, and each app depends on a single provider.

- **One provider means one point of failure.** Trackers built on AniList or MyAnimeList stop working when that service does; on 21 October 2026 AniList took its site and public API offline over a PHP security vulnerability.
- **No provider covers everything.** AniList tracks anime and manga at best; visual novels and games live elsewhere.

## What Yumeniwa does

- **Spreads the risk.** Your data lives in a *Local Store* on every device you use, backed up to Google Drive and synced through a *Central Store*, in the spirit of Git and GitHub.
- **Aggregates providers.** One library across media types, fetched from several providers. Version 1 ships with a tested set of providers; *bring your own provider* follows once the core works.
- **Syncs both ways where it can.** Changes go back to providers that allow write access; the ones that don't are listed openly.
- **Works without a provider.** Add *manual* records yourself. They are never sent to providers, but they sync across your devices like everything else.

## Stack

MongoDB, Express, React and Node (JavaScript, ES modules), packaged as a PWA for PC and Android.

## Later

- Social features: forums, discussion groups, rich reviews.
- A taste profile with deeper analytics and AI-assisted recommendations.
- Built-in viewers for anime, manga and light novels, tracking as you watch or read.

---

Built from scratch as a learning project: the design and every line of application code are written by hand. Research assisted by Claude.

Yumeniwa started as the tracker I wanted for myself and couldn't find. If it ends up being yours too, I'd love to hear about it.

We hope you enjoy it :)
