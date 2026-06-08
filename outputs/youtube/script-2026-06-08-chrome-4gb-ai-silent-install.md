# YouTube Script Outline — 2026-06-08
**Topic:** Chrome's 4GB silent AI install
**Slug:** chrome-4gb-ai-silent-install

---

**Title A (curiosity gap):** "Your computer has a 4GB AI file on it. You didn't put it there."
**Title B (direct):** "How Google Chrome silently installed an AI model on your device"
**Estimated runtime:** ~5.5 minutes at natural narration pace (~130 wpm / ~720 words of spoken content)

---

## HOOK — first 15 seconds

Open your file manager and search for a file called weights.bin. Four gigabytes. You didn't download it. Google Chrome put it there — automatically, in the background, without telling you. And if you found it and deleted it, Chrome downloaded it again.

---

## SETUP — the problem stated plainly

This is a story about a decision Google made: that your hard drive is a reasonable place to store its AI software, and you don't need to be consulted about it.

Chrome is the most-used browser on the planet. Roughly two out of every three desktop computers are running it right now. Starting sometime in 2025 and continuing through 2026, Chrome began silently downloading Gemini Nano — Google's on-device AI model — onto qualifying devices.

No notification. No opt-in. No storage warning. Just a 4GB file, placed in a folder called OptGuideOnDeviceModel, because Google's systems determined your hardware could support it.

When a security researcher found it in May 2026 and published the details, the story spread fast — partly because users reported it had been happening for nearly a year, with no one being told. [VERIFY THIS — confirm original discovery timeline]

---

## EXPLANATION — what's actually happening

What is Gemini Nano? It's a compressed AI model designed to run locally on your machine rather than on a remote server. Google's reasoning here is actually defensible: local processing means your input doesn't have to travel to a data center. The writing assist feature that appears in text forms on websites? That uses Gemini Nano. It stays on your device.

The problem isn't what the model does. The problem is that Google decided to install it first, and not mention it.

Google did eventually add a settings toggle — in early 2026 — that lets you disable the feature and remove the model file. [VERIFY THIS — confirm the toggle exists and the exact path in current Chrome] But that toggle doesn't announce itself either. You have to go find it.

---

## NUANCE — the thing most coverage got wrong

Here's what most explainers on this topic missed, or got backwards.

Chrome has a visible AI Mode button in the address bar — a small icon that activates an AI-powered search experience. You now know Chrome has a local AI model installed on your machine. The natural assumption is that AI Mode uses that local model. Your searches stay on your device. Private.

That assumption is wrong.

AI Mode routes your queries to Google's cloud servers. It's powered by Google's Search Generative Experience backend — the same infrastructure that's been behind Chrome's AI search features for a while. The local Gemini Nano model powers a separate, narrower category of features. Writing assist. Certain background tasks. Not the AI search experience with the prominent button. [VERIFY THIS — confirm AI Mode is definitively cloud-routed and not hybrid]

So: the feature that looks like it's keeping your data local is the cloud one. The file that feels alarming is actually the more private one. Both things are true at the same time.

This isn't reassuring, exactly. It just means the concern is aimed at the wrong target. The file took up space you didn't consent to give. And the prominent AI feature in the address bar is sending your queries to Google either way.

---

## TAKEAWAY — one clear thing to do

If you want to check whether the file is there: on Windows, look in AppData > Local > Google > Chrome > User Data > OptGuideOnDeviceModel. On Mac, it's in Library > Application Support > Google > Chrome > OptGuideOnDeviceModel. [VERIFY THIS — confirm current paths for Chrome 147+]

To prevent the redownload: Chrome Settings > Privacy and Security > AI features > turn off "Use AI features." [VERIFY THIS — exact menu path in current Chrome version]

If you'd prefer a browser that doesn't do this, Firefox and Brave are both worth considering. Same websites work. Free. No gigabyte AI models being deposited on your disk without your knowledge. [VERIFY THIS — confirm neither currently has equivalent silent install behavior]

The thing to carry with you: local AI and private AI aren't the same thing. A model running on your device isn't necessarily safer than one running in the cloud — it depends entirely on what data it touches and where the results go. The file that showed up without permission is the less concerning one. The button that looks private isn't. That distinction is worth knowing.

---

*Production notes: No B-roll of AI imagery — consider screen recording of the actual file path and settings toggle instead. Keep graphics tight and functional.*
