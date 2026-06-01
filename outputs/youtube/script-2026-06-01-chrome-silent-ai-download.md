# YouTube Script Outline — Topic #1
**Date:** June 1, 2026
**Topic slug:** chrome-silent-ai-download

---

**Title variant A (curiosity gap):** Google put a 4GB AI on your computer. You didn't ask.
**Title variant B (direct):** Chrome's Silent AI Installation: What It Is and How to Remove It
**Estimated runtime:** ~5.8 minutes at natural narration pace (~130 words/minute)

---

## HOOK — First 15 seconds

Go to your Chrome browser right now. In the address bar, type: `chrome://on-device-internals` — press enter.

If you see the words "model available" with a file path — there's a 4-gigabyte AI model on your computer. Google installed it. You didn't ask for it.

[VERIFY THIS — confirm this URL and what a non-technical user actually sees when they navigate to it in current Chrome]

---

## SETUP

This has been happening quietly for months. Chrome — used by a significant majority of people on the planet — has been downloading and installing Google's on-device AI model onto qualifying computers automatically. No notification. No opt-in prompt. And if you find the file and delete it, Chrome reinstalls it.

We're going to cover what this model actually is, what it does, whether you need to worry, and what you can do about it.

---

## EXPLANATION

The model is called Gemini Nano — it's the smallest model in Google's Gemini AI family. "Small" is relative here: it's a 4-gigabyte file called `weights.bin`, stored inside a folder in your Chrome profile directory called `OptGuideOnDeviceModel`. Google installed it because your machine met the hardware requirements — enough RAM, enough storage.

What does it do? Google uses it for three things right now: a text composition assistant called "Help me write," an on-device scam detection feature that flags sketchy web pages, and something called the Summarizer API.

That last one is worth flagging specifically. The Summarizer API isn't just a feature you use — it's a tool that websites you visit can call directly, using your device's processing power to summarize content on their behalf. Your hardware, their feature. [VERIFY THIS — confirm Summarizer API access for third-party sites vs. Chrome-only usage]

Security researcher Alexander Hanff documented this installation behavior, the story got wide attention in May 2026, and Google confirmed it. Google says they added a setting to turn it off and remove the model — but the rollout of that setting is still uneven. Not everyone has access to it yet. The default, unless you've specifically found and changed this setting, is still: model installed.

---

## NUANCE — The thing most explainer videos on this topic skip

Here's where I want to give you the honest picture, because a lot of coverage of this story stops at "Google bad."

On-device AI is actually better for privacy than the cloud alternative. When the model runs locally on your machine, Google isn't receiving a request every time you use one of these features. The data stays on your device. Apple has been making this exact argument about its own AI features for a couple of years now.

In a narrow technical sense, Google made a privacy-positive engineering choice.

The problem is they made it for you. On your hardware. Without asking. And they designed it to come back when you remove it.

[YOUR TAKE ON THIS — worth a beat here on the "good outcome, bad process" tension. The privacy benefit is real. The consent violation is also real. Both things are true simultaneously.]

"Better than the cloud version" is not the same thing as "you agreed to this." Those are different conversations. What's missing isn't the technology — it's the baseline respect for your ability to choose.

This is worth naming because the privacy-forward argument will be Google's defense, and it's not entirely wrong. It's just also not the point.

---

## TAKEAWAY

Two things to do right now.

First: type `chrome://on-device-internals` into Chrome to see if the model is installed on your device. If you see "model available" with a file path, it's there.

Second: go to Chrome Settings → then Privacy and Security → then AI features. If you see a toggle related to on-device AI, you can turn it off and remove the model from your device. [VERIFY THIS — confirm the exact settings path and toggle label in current Chrome builds, and whether it actually removes the existing file or only prevents future downloads]

If that setting isn't visible in your Chrome, you're not in the rollout group yet and your options are limited to waiting for the setting or switching browsers.

If you want a browser where AI features are opt-in by default rather than installed automatically, Privacy Guides at privacyguides.org has current comparisons. Firefox and Brave handle this differently and are worth a look.

The bigger-picture takeaway: your browser is now an active layer in how AI operates on your device — it can run models, it can serve as infrastructure for website features, it can use your hardware for things you haven't specifically requested. Knowing that your browser is making these decisions is the starting point for making your own.

---

*[No subscribe/like/bell call-to-action — per brand voice guidelines]*
