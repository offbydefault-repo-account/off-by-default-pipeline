# YOUTUBE SCRIPT OUTLINE
**Date:** 2026-05-25
**Topic:** Chrome's silent AI install
**Slug:** chrome-ai-secret-install

---

**Title A (curiosity gap):** "Google secretly put a 4GB AI on your computer. Here's what to do."
**Title B (direct):** "Google Chrome's hidden AI download, explained"
**Estimated runtime:** ~6 minutes (750 words ÷ ~130 words per minute at natural pace)

---

## SCRIPT OUTLINE

---

### HOOK — first 15 seconds

"There's a 4-gigabyte file sitting on your computer right now that you didn't download. You weren't asked. You didn't get a notification. Google's Chrome browser just... put it there. And if you deleted it without knowing what it was, Chrome re-downloaded it the next time you opened the browser."

*(pause)*

"I want to show you exactly what it is, what it does, and how to make it stop."

---

### SETUP — the problem, plainly stated

Chrome has been silently installing a local AI model — called Gemini Nano — onto computers running recent versions of the browser. This started rolling out in early 2026. It affects modern computers that meet certain hardware requirements, which is most of them.

Most users have no idea this happened. The file doesn't show up in your downloads. There's no notification in the browser. Chrome treats it as part of its own internal infrastructure, not a feature you chose.

The file is 4 gigabytes. That's roughly the size of a full HD movie.

---

### EXPLANATION — the actual answer in plain language

**What Gemini Nano is:**
It's Google's on-device AI model — a stripped-down version of their AI system designed to run locally on your hardware, without sending data to Google's servers. Chrome uses it to power three things:

- A "Help me write" suggestion tool that appears when you're typing in a text field
- An on-device scam detection feature that looks for red flags on pages you visit
- A summarization API that website developers can call from their own sites

**Why Google says it's a privacy feature:**
The "on-device" framing is intentional. Google's argument is that running AI locally — on your machine, not their servers — means your activity doesn't go back to Google. That argument has real merit. There is a meaningful difference between processing happening on your laptop versus in a cloud log.

**Where that argument breaks down:**
The privacy argument would be more convincing if they'd asked first. A feature that installs itself without consent, that reinstates itself after you delete it, and that required a settings toggle to stop — is doing something that, in any other context, we'd call unwanted software behavior.

**How to check if you have it:**
Type `chrome://components` in your browser address bar. Look for "Optimization Guide On Device Model." If it's there, it shows you the version number and file size. That's your confirmation.

*(show screen if filming: chrome://components page, highlight the entry)*

**How to remove it:**
Open Chrome Settings, search for "AI" or "on-device" in the settings search bar, find the option to disable the on-device AI model, and turn it off. With that disabled, Chrome stops reinstalling the file. Then you can navigate to the folder — on Windows it's `%LOCALAPPDATA%\Google\Chrome\User Data\OptGuideOnDeviceModel` — and delete what's there.

[VERIFY THIS — settings path may vary slightly by Chrome version; test on current stable release before filming]

---

### NUANCE — what most explainer videos on this topic skip

Most coverage landed on "Google is spying on you." That's not quite what happened, and it's worth being precise.

The Gemini Nano model runs on your hardware. It doesn't send your keystrokes or browsing to Google. That's a real distinction.

The more accurate concern is about consent architecture — who makes decisions about what gets installed on your machine, and when. Google made a choice about your disk space, your bandwidth, and your hardware resources without your knowledge. That's the issue.

There's also a quiet double standard worth naming: if any other software company downloaded a 4GB file to your machine without asking, installed it as part of a routine update, and made it re-download when you deleted it — we'd call that a security threat. When a browser maker does it with their own AI model, it gets called a rollout.

The scam detection feature, for what it's worth, is genuinely useful. If they'd announced it and asked, a lot of people would have said yes. They chose not to ask.

[HUMOR OPPORTUNITY? — FLAG FOR REVIEW: something about the world's most politely worded opt-out for something that already happened]

---

### TAKEAWAY — one clear thing to remember or do

Type `chrome://components` into Chrome and look at what your browser has installed on your behalf. It lists every component Chrome has written to your system — not just the AI model, but everything. It's the closest thing Chrome has to a nutrition label, and it's not something they advertise.

If you don't want the AI model on your machine, the steps are simple: turn it off in settings, then delete the folder. Five minutes.

If you do want it — or you're fine with it — you don't need to do anything. The model runs locally. Just know it's there.

---

*[End of outline — no subscribe CTA, no bell reminder]*

---

*Script outline word count: ~680 words. Estimated runtime at 130 wpm: ~5.5 minutes. Expand the EXPLANATION section with on-screen demos and pauses to reach 6 minutes.*
