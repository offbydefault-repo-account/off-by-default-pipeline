# Newsletter Draft — 2026-05-18
**Topic:** Chrome's Gemini Nano silent install

---

**Subject line A (curiosity gap):** Your browser downloaded something. You didn't ask it to.
**Subject line B (direct):** What Google quietly installed on your computer — and how to check
**Social summary:** Google Chrome silently downloaded a 4GB AI model to hundreds of millions of computers without asking. Here's what it is, whether it's on yours, and how to remove it.

---

Somewhere on your computer, there's a file you didn't put there. It's called `weights.bin`. It's 4 gigabytes. And if you use Google Chrome — which two out of every three people on the internet do — it's probably sitting there right now.

Google put it there. They didn't ask. They didn't notify you. And if you delete it, Chrome downloads it again automatically.

This is not a security breach. This is not a bug. This is a decision Google made — to install its AI model on a billion devices without a single consent screen.

---

The file is the Gemini Nano model, Google's on-device artificial intelligence. It lives inside your Chrome profile folder, in a directory called OptGuideOnDeviceModel. It powers three Chrome features: a "Help me write" button that appears in text fields on some websites, an on-device scam detection system for calls and messages, and something called the Summarizer API — a tool that lets websites call the AI model directly from your browser.

Gemini Nano is what's called a "local" AI model. Unlike typing something into ChatGPT or Gemini.com, when Nano runs, it runs on your machine — your processor, your memory, your storage. Google has leaned on this in their public statements, describing it as better for privacy because your prompts don't travel to their servers. That part is accurate.

What that framing skips is the part where you never agreed to host the model in the first place. [YOUR TAKE ON THIS]

Researchers first noticed the file in early May 2026, when someone spotted an unexplained 4GB file in their Chrome profile and started asking questions. The story spread fast — Hacker News, Reddit, Slashdot — and within days, hundreds of users had confirmed the same file on Windows, macOS, and Linux machines. Google confirmed it was intentional.

[PERSONAL EXAMPLE — did you find this on your machine? What did it feel like to discover it was there?]

---

In February 2026, Google added a toggle to Chrome settings that lets you disable the model and stop it from redownloading. The toggle is real, and turning it off works. But the sequence matters: the model was installed before the toggle existed, on hundreds of millions of devices, without notification. Google built the opt-out after the rollout, not before it.

That's the part that deserves more attention than the storage number. Most people have more than 4GB free. The 4GB isn't really the issue.

The issue is that Chrome — a piece of software most people think of as a neutral tool, like a window to the internet — turned out to be something Google uses to install its products on your machine. You didn't download Chrome thinking you were agreeing to be part of a billion-device AI rollout. But that's what happened.

Here's the counterintuitive part: the fact that the model runs locally might actually be the most honest version of what's coming. Every major browser vendor is building AI features into the browser itself. The question of whether there's a 4GB model file on your device isn't the long-term issue — the long-term issue is who controls what software runs on hardware you paid for.

[HUMOR OPPORTUNITY? — FLAG FOR REVIEW — something about the "Help me write" feature and whether the storage cost is worth it for a button you've never clicked]

There's a scale problem here that individual privacy doesn't capture. Across a billion Chrome installs, pushing 4GB of model weights — even once — generates an estimated 6,000 to 60,000 tonnes of CO2 equivalent emissions depending on the energy mix. [VERIFY THIS — range is from environmental researchers, confirm the primary source before publishing] For users in countries where 4GB represents a full month's mobile data plan, Chrome consumed that allowance without warning. None of those users were asked. [SOURCE NEEDED: data on countries where 4GB is equivalent to a monthly mobile plan — look for Statista or GSMA data]

---

Here's what you can do right now.

To check if the file is on your machine: on Windows, type this into your file explorer address bar: `%LOCALAPPDATA%\Google\Chrome\User Data\OptGuideOnDeviceModel\` — look for a file called `weights.bin`. On Mac, the folder is inside `~/Library/Application Support/Google/Chrome/`. [VERIFY THIS — confirm Mac and Linux paths before publishing]

To turn it off: open Chrome, go to Settings, click "System" in the left sidebar, and look for the "On-device AI" toggle. Turn it off. Google says this stops the model from running and prevents automatic redownloads.

If you want to see Chrome's full storage footprint, type `chrome://settings/storage` into the address bar. It won't give you granular control, but it shows you what Chrome is using your disk for.

California's AB 2561 — which passed the state Assembly unanimously this week — would require apps and operating systems to default to the most privacy-protective setting available, and would prohibit them from changing your privacy settings without explicit consent. [VERIFY THIS — confirm it hasn't stalled in Senate] If it becomes law, what Chrome did this year would be illegal in California going forward. That doesn't fix today's situation. But it tells you where the legislative pressure is pointing.

---

**One resource:** If you want a browser that doesn't do this — Brave is built on the same Chromium engine as Chrome, runs all the same extensions, but doesn't have Google's AI pipeline baked in. [YOUR TAKE ON THIS — is Brave your actual recommendation, or is there a caveat worth naming?]

---

The 4GB file is easy enough to delete. The harder question — who gets to decide what runs on a device you own — doesn't have an easy answer yet.

---

*Word count: ~880 words*

---

**Affiliate opportunity:** Brave browser (free, no referral program but honest recommendation). If Off by Default has a VPN partner, a brief note that a VPN doesn't stop this particular issue — so only recommend if it genuinely applies to other topics in this issue.
