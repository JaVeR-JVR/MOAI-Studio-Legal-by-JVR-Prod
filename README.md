# MOAI Studio 21 🗿🎛️
 
**MOAI Studio 21** is a tiny, unserious Discord Rich Presence project from **JVR_Prod**. Its mission is simple: make the profile say something other than “Online” and let the MOAI cook.

> **MOAI make BRrrrAM BAM BAM BA-Bam in MOAI Studio = MOAI hapy)))**
>
> One developer. Zero Grammy nominations. Infinite stone-face energy.

[Terms of Service](terms.html) · [Privacy Policy](privacy.html) · [Русская версия README](README.ru.md)

## What is MOAI Studio 21?

It is a joke project inspired by the naming energy of **FL Studio 21**, internet music-production memes, and the 🗿 MOAI reaction: expressionless face, questionable decisions, immaculate vibes.

The “21” is a playful nod to FL Studio 21. **MOAI Studio 21 is an independent parody project and is not affiliated with, endorsed by, or sponsored by Image-Line or FL Studio.** It is also not affiliated with Discord.

The idea is not to build the next industry-standard digital audio workstation. The idea is to put a funny, custom activity on a Discord profile. If the MOAI is happy, the mix is finished. If the mix is clipping, the MOAI remains calm.

## How it works

MOAI Studio 21 uses Discord Rich Presence as its identity/display configuration. Rich Presence is the feature that lets a compatible application send activity information to the running Discord desktop client.

1. **Application identity.** The project is registered in the Discord Developer Portal and has an Application ID. Artwork used by the activity can be uploaded as application assets.
2. **Local RPC client.** A compatible Rich Presence client runs on the same computer and prepares the activity text, timestamps, and image asset keys.
3. **Local connection.** The client communicates with the running Discord desktop app through Discord's local RPC interface (IPC).
4. **Discord displays the bit.** Discord renders the activity using the data and assets it receives, subject to Discord's own behavior and the user's activity/privacy settings.
5. **Stop the bit.** When the RPC client clears or stops updating the activity, the custom presence is no longer maintained.

**Important reality check:** the Application ID is an identifier, not a magic executable. Changing the app name in the Developer Portal does not create an RPC client. This repository contains the project website, legal pages, and documentation; it does **not** contain a standalone desktop app or RPC client.

## The MOAI production workflow

- Open Discord.
- Start your compatible Rich Presence client.
- Set the activity fields to something musically responsible, such as:
  - **Details:** `MOAI is cooking the 808`
  - **State:** `Sidechain? I hardly know her`
  - **Image tooltip:** `Certified boulder moment`
- Admire the profile card like it just got a Reddit “this goes hard” comment.
- Remember: if the master is red, that is not a mastering technique. Probably.

## Features (spiritually speaking)

- 🗿 **MOAI-grade branding** — stone-faced, bass-heavy, emotionally unavailable.
- 🎹 **FL Studio 21-inspired naming** — a respectful nod to DAW culture, not an official product.
- 💿 **Producer meme vocabulary** — 808s, sidechain, clipping, “one more plugin,” and the sacred unfinished loop.
- 🕒 **Rich Presence fields** — the exact fields available depend on the RPC client you use.
- 🧍 **Solo-dev production** — built by one developer under the JVR_Prod name. The team meeting fits in one chair.

## Repository contents

| File | Purpose |
| --- | --- |
| `index.html` | Landing page linking to the legal documents |
| `terms.html` | Terms of Service |
| `privacy.html` | Privacy Policy |
| `README.md` | Project overview (English) |
| `README.ru.md` | Project overview (Russian) |
| `DEPLOYMENT_RU.txt` | Russian GitHub Pages publishing instructions |

## Privacy and data handling

This repository is a static website. It does not implement a user account system, application backend, or analytics of its own. In the intended Rich Presence setup, the local RPC client sends configured activity data to Discord so Discord can display it. Discord processes that information under its own terms and privacy policy.

Third-party RPC clients may have their own permissions, logs, telemetry, or data practices. Those are not controlled by this repository; check the client you choose. The Privacy Policy is accurate only while the project does not independently collect or store personal information through a backend. If that changes, update the policy before deploying the change.

## Publish the legal pages with GitHub Pages

1. Create a **public** GitHub repository (for example, `moai-studio-21`).
2. Upload `index.html`, `terms.html`, and `privacy.html` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**, choose the `main` branch and `/(root)`, then save.
5. Wait for deployment and verify that all pages open publicly without signing in.
6. Add the published `terms.html` and `privacy.html` URLs to the matching fields in Discord Developer Portal → **General Information**.

The URLs will look like this (replace `YOUR-GITHUB-USERNAME` with your GitHub username):

- `https://YOUR-GITHUB-USERNAME.github.io/moai-studio-21/`
- `https://YOUR-GITHUB-USERNAME.github.io/moai-studio-21/terms.html`
- `https://YOUR-GITHUB-USERNAME.github.io/moai-studio-21/privacy.html`

## References

- [Discord Rich Presence overview](https://discord.com/developers/docs/rich-presence/overview)
- [Discord RPC documentation](https://discord.com/developers/docs/topics/rpc)
- [Discord Privacy Policy](https://discord.com/privacy)
- [FL Studio](https://www.image-line.com/fl-studio/)

## Disclaimer

MOAI Studio 21 is an independent parody project created by **JVR_Prod**, maintained by one developer. It is not affiliated with, sponsored by, or endorsed by Discord Inc., Image-Line, or FL Studio. Discord, FL Studio, and related names/logos are the property of their respective owners.

This README explains the intended setup, not a promise that every RPC client or Discord version will behave identically. Legal pages are practical project documents, not legal advice. Memes are for vibes; please do not master your actual mix by reading this README.
