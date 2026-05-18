# YouTube Script Outline — 2026-05-18
**Topic:** Chrome's Gemini Nano silent install

---

**Title A (curiosity gap):** Google installed a 4GB AI on your computer. You didn't ask.
**Title B (direct):** What Chrome's hidden AI file does — and how to remove it
**Estimated runtime:** ~5:45 at natural narration pace (~130 words/minute)

---

## HOOK — First 15 seconds

There's a 4-gigabyte file on your computer that you didn't put there. It's on your laptop, your desktop, probably both. Google put it there. They didn't ask. And if you've already deleted it — it came back.

Here's what it is, what it does, and how to actually get rid of it.

---

## SETUP

Google Chrome has been quietly downloading its Gemini Nano AI model onto users' devices since late 2025. The model file is called `weights.bin`, it's 4 gigabytes, and it lives inside your Chrome profile folder in a subdirectory called OptGuideOnDeviceModel.

Researchers noticed this in early May 2026. One person spotted an unexplained file eating up storage, started asking questions online, and within hours hundreds of users had confirmed the same thing on Windows, Mac, and Linux. Google confirmed it was intentional.

Two out of every three people on the internet use Chrome. That's roughly a billion devices. None of them got a dialog box asking if this was okay.

---

## EXPLANATION — What is this file and what does it do?

Gemini Nano is an on-device AI model — meaning it runs on your computer, not Google's servers. When it processes something, your text doesn't leave your machine. That's different from using ChatGPT or Google's Gemini website, where everything you type goes to a server somewhere.

The model powers three things in Chrome right now. First: a "Help me write" button that appears in text boxes on some websites. Second: an on-device scam detection feature for calls and messages. Third: something called the Summarizer API, which lets websites call the AI model from inside your browser.

Here's how to check if it's on your machine.

On Windows, open File Explorer and type this into the address bar: `%LOCALAPPDATA%\Google\Chrome\User Data\OptGuideOnDeviceModel\` — if there's a `weights.bin` file there, it's installed. On Mac, look inside `~/Library/Application Support/Google/Chrome/` for the same folder. [VERIFY PATHS — confirm Mac/Linux before recording]

To remove it and keep it off: open Chrome Settings, go to System in the left sidebar, find "On-device AI," and toggle it off. Google says that stops the model from running and prevents the automatic redownload.

[⚠ REWRITE — SOUNDS GENERATED] — if any of the path instructions sound overly formal on camera, punch them up with your natural explanation style.

---

## NUANCE — The thing most explainers get wrong

Most of the coverage on this has focused on the 4 gigabytes. "They stole your storage." That's real, and it matters in some cases — especially for people in countries where 4GB is literally a full month of mobile data. But for most people watching this, 4GB isn't the actual issue.

The issue is what this reveals about Chrome itself.

You think of your browser as a neutral tool. A window. Something you use to visit the internet. It doesn't feel like software that installs other software.

But Chrome is a Google product, and Google used it to deploy its own AI infrastructure onto a billion machines without announcing it. That's not a bug in how Chrome works — it's a feature of what Chrome actually is. It's distribution infrastructure. Google already installed Chrome. Then Google used Chrome to install something else.

The local processing is, in one sense, a real privacy benefit — your prompts don't go to Google when Nano runs. But that framing skips over the part where you never agreed to be part of this rollout. Privacy-preserving and consent-free are not the same thing. They made it local so it's better for you. They made it silent because asking would have gotten in the way.

Also worth knowing: Google didn't add a toggle to turn this off until February 2026 — after the model had already been deployed to hundreds of millions of devices. They built the opt-out after the rollout, not before it.

[YOUR TAKE ON THIS — is there something specific about this sequence that you find particularly frustrating or clarifying?]

---

## TAKEAWAY

One thing to remember from this: your browser is not a neutral tool. It is a product made by a company that has interests, and those interests include getting their AI onto as many devices as possible. That's not a conspiracy — it's just what browser vendors do now. Chrome, Edge, and others are all building AI features directly into the browser layer.

The toggle to disable Gemini Nano is real and it works. Turn it off if you want. But the more durable question is: which software do you actually want making decisions about what lives on your machine?

[YOUR TAKE ON THIS — is there a browser you genuinely recommend? Brave is the natural answer here, since it's Chromium-based and doesn't do this. Only say so if you mean it.]

---

*Script word count: ~720 words | Runtime: ~5:30*

---

**Production notes for Kelly:**
- The file path on-screen graphic would help a lot here — text on a black background showing the Windows path
- The Chrome settings toggle walkthrough could be a brief screen recording if you want to show it live
- Thumbnail: screenshot of the weights.bin file with a "you didn't ask for this" caption tends to perform well for privacy-anxiety content
