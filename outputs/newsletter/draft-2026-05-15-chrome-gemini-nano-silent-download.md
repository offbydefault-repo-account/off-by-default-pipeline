# NEWSLETTER DRAFT — Issue #1
**Date:** 2026-05-15
**Topic:** Google Chrome's silent Gemini Nano installation

---

**Subject line A (curiosity gap):** Something is quietly living on your hard drive. Here's what it is.
**Subject line B (direct):** Google put a 4GB AI file on your computer without asking

**Social distribution summary:** Google Chrome has been silently downloading a 4GB AI model to user devices — no opt-in, no notification — and it reinstalls itself automatically if you delete it.

---

## DRAFT BODY

Your computer has a new file on it. You didn't put it there. You weren't asked. And if you find it and delete it, it comes back.

If you use Google Chrome — which is roughly two out of every three internet users — there's a very good chance this file already exists on your machine. It's 4 gigabytes. It lives inside a folder called `OptGuideOnDeviceModel`. The file itself is called `weights.bin`. These names are not accidents. They're the kind of deliberately unrecognizable bureaucratic naming that says: please don't go looking for this.

What the file contains is a complete copy of Gemini Nano, Google's on-device artificial intelligence model. It was downloaded to your device through a routine Chrome update at some point in the past year. There was no pop-up. No opt-in screen. No email. You probably have it right now and have no idea.

---

**What Gemini Nano actually is** — and why Google says this is fine

Gemini Nano is a smaller, stripped-down version of Google's AI. Unlike the AI you'd access through gemini.google.com, this one runs entirely on your device. Your processor does the work. Nothing gets sent to Google's servers. Google frames this as a privacy feature: your data stays local.

That argument has some real merit. On-device AI processing is genuinely different from cloud-based processing. When a model runs locally, there's no server receiving your inputs, no cloud log of your text. In certain threat models, this is meaningfully more private.

But the privacy argument and the consent argument are two entirely separate conversations. And Google has been conflating them. Whether on-device AI is more private than cloud AI is one question. Whether you agreed to have 4 gigabytes of Google's software installed on your machine is a different question. The first doesn't answer the second.

---

**What the model actually does — including the part most coverage skipped**

The Gemini Nano model powers a few Chrome features you may have encountered. "Help me write" — the button that appears when you right-click inside a text field — runs on it. There's on-device scam detection, which flags suspicious websites before they load. And there's the Chrome Summarizer API.

The Summarizer API is the part worth pausing on. It's a programming interface that any website — not just Google products, not just Chrome features — can call directly. When you visit a website that has implemented the Summarizer API, that site can trigger the AI model sitting on your computer. Your processor does the work. Your storage hosts the model.

You are not just running this for Google's convenience. You are hosting AI infrastructure that the broader web can use, on behalf of websites you've never heard of, without having agreed to any of that. [⚠ REWRITE — SOUNDS GENERATED] [YOUR TAKE ON THIS — is the Summarizer API angle overstated, or is this genuinely a meaningful shift in how websites can use your hardware?]

---

**Who caught this and what they said**

A privacy researcher named Christian Hanff — a computer scientist and lawyer based in Europe — publicized this in early May 2026. He verified the behavior by checking macOS kernel filesystem logs, confirmed the model downloads automatically on Windows, Mac, and Linux, and filed a formal complaint arguing that Chrome's behavior violates the EU's ePrivacy Directive. [VERIFY THIS — confirm Hanff filed formally with a specific regulatory body, not just published a public complaint]

The ePrivacy Directive requires explicit user consent before software is installed on a user's device. Hanff's argument is that model weights — even if they run locally — constitute software being installed. Google hasn't publicly responded to that characterization as of this writing. [VERIFY THIS — check for any Google statement responding to Hanff or the controversy]

Hanff also calculated the carbon cost. Distributing 4 gigabytes to somewhere between 500 million and 1 billion Chrome users accounts for an estimated 6,000 to 60,000 metric tons of CO2 — just for the download, before any of those models ever run. [VERIFY THIS — confirm Hanff's methodology and the 500M–1B estimate is reasonable for Chrome's user base]

---

**The part that answers the "so just delete it" response**

You can delete the file. The path on a Mac is `~/Library/Application Support/Google/Chrome/` — look for the `OptGuideOnDeviceModel` folder inside. On Windows, it's in `C:\Users\[your username]\AppData\Local\Google\Chrome\User Data`. [VERIFY THIS — test on current Chrome versions to confirm folder location accuracy]

If you delete it, Chrome downloads it again. This isn't a bug. It's a product decision. The browser was built to maintain this model on your device regardless of whether you want it there.

There are Chrome flags — experimental settings accessible by typing `chrome://flags` into your address bar and searching for "Gemini Nano" — that may disable the features powered by the model. Whether disabling the features also stops the download is not confirmed. [VERIFY THIS — test or find a reliable source confirming whether flags prevent re-download]

Enterprise IT administrators have complete controls for this through Chrome's management policies. Individual users, currently, do not have a clean opt-out. [VERIFY THIS — confirm there's no user-facing opt-out in Chrome settings]

---

**What you can do now**

Check whether the file is on your machine. The paths above take about two minutes to navigate. Knowing what's there is better than guessing.

If you want to try disabling Gemini Nano features, the flags route is your current option, with the caveat above about whether it fully works.

The more substantial decision is whether this changes how you feel about Chrome. A browser that installs things without telling you — and reinstalls them when you remove them — has made a clear choice about whose preferences take priority. Firefox doesn't do this. Switching browsers isn't a small ask, and it's reasonable to weigh the friction against how much this actually bothers you. [YOUR TAKE ON THIS — is recommending Firefox too aggressive here, or is it the appropriate call given the facts?] [PERSONAL EXAMPLE — do you use Chrome? Have you checked for this file?]

---

**One recommendation:**
Check the folder path for your operating system. Right now, before you close this. If the file is there, you've answered the question. What you do with that answer is up to you.

---

**Closing line:**
The file reinstalling itself isn't an oversight. It's a policy — one that tells you, quietly, whose computer Google thinks this is.

---

*Suggested affiliate opportunity: None forced. If Kelly has a Firefox partnership or a privacy-focused VPN affiliate, this issue creates a natural placement. Do not manufacture one.*

---

**[VERIFY THIS] flags in this draft:**
1. Confirm Hanff filed formally with a specific EU regulatory body (vs. public post only)
2. Confirm Google has not issued a formal public response as of May 15, 2026
3. Confirm folder paths for OptGuideOnDeviceModel are accurate across Chrome versions on Mac/Windows/Linux
4. Confirm whether Chrome flags prevent re-download or only disable features
5. Confirm there is no user-facing opt-out in standard Chrome settings (non-enterprise)

---
*Word count: ~950 words body*
