# YOUTUBE SCRIPT OUTLINE — Video #1
**Date:** 2026-05-15
**Topic:** Google Chrome's silent Gemini Nano installation

---

**Title variant A (curiosity gap):** Google Put Something on Your Computer Without Asking
**Title variant B (direct):** What Google Chrome's Hidden 4GB AI File Actually Does — And How to Find It

**Estimated runtime:** ~750 words at natural narration pace (~130 words/minute) ≈ **5 minutes 45 seconds**

---

## SCRIPT OUTLINE

---

### HOOK — First 15 seconds

*Speak directly to camera, no intro card yet.*

"If you use Google Chrome, there's probably a four-gigabyte file on your computer right now that you never agreed to download. I'm going to show you exactly where to find it, what it does, and what your options actually are."

*[Cut to screen recording of the folder path opening on Mac or Windows — show the file existing before any explanation.]*

---

### SETUP — The problem, stated plainly

Most people know Chrome updates automatically. Security patches, bug fixes — that's normal browser behavior, and most of it is genuinely useful. This is different.

What Google has been distributing through Chrome isn't a patch or a cached resource or an updated dictionary. It's a complete machine learning model. The full set of parameters Google uses to run an AI — every numerical weight that defines how the model thinks — installed on your machine through a routine update, without a prompt, without a notification, without an opt-in.

The folder is called `OptGuideOnDeviceModel`. The file inside it is called `weights.bin`. These names were clearly not chosen to be obvious. There's nothing here that would tell a normal person: this is a 4-gigabyte AI that Google installed on your computer.

*[Show the folder on screen. Point out the file name. Let it land.]*

---

### EXPLANATION — The actual answer, in plain language

**What is it?**
This is Gemini Nano — Google's on-device language model. "On-device" means it runs directly on your processor. It doesn't send your inputs to Google's servers. The AI processing happens locally.

**What does it actually do?**
Three things, currently. First: it powers the "Help me write" feature in Chrome — the one that appears when you right-click inside a text box and offers to generate or improve what you're typing. Second: it runs Chrome's on-device scam detection, which evaluates websites for suspicious patterns before they fully load. Third: it powers something called the Summarizer API.

*[Pause on the third point.]*

The Summarizer API is the one most coverage on this story missed. It's not a Chrome feature. It's a programming interface — a tool that any website can build into itself and call directly. When you visit a website that has implemented the Summarizer API, that site can trigger the model sitting on your computer. Your processor does the work. Your storage is what Google installed the model onto.

You're not just running this AI for Google's convenience. You're hosting infrastructure that the broader web can activate, without having agreed to any of that. [VERIFY THIS — confirm the Summarizer API is accessible to third-party sites and document a real example]

**Why does Google say this is fine?**
Their argument is privacy: on-device AI is more private than cloud AI because nothing leaves your machine. That's a real argument. On-device processing does eliminate certain privacy risks.

But that's the wrong question. The privacy architecture of the model and the consent architecture of the model are two different things. You can have an AI that runs locally *and* that you agreed to have installed. Google chose to do only the first part.

---

### NUANCE — The thing most explainer videos on this topic skip

*[Direct to camera, slower pace.]*

A lot of the coverage on this story presents it as: "Google put AI on your computer, but it's okay because it's private." That's Google's framing, and it's doing a lot of work.

Here's what that framing skips: the file reinstalls itself if you delete it.

That's not an accident. That's not an oversight in the code. Someone at Google made a product decision that says: if a user finds this and removes it, restore it. That decision was made deliberately, and it tells you something. When a piece of software is designed to resist removal, the people who built it knew it would face resistance.

A researcher in Europe — Christian Hanff, a privacy advocate and computer scientist — filed a formal complaint arguing this violates EU privacy law. [VERIFY THIS — confirm formal complaint vs. public letter] He calculated that distributing 4 gigabytes to somewhere between 500 million and 1 billion Chrome users produces between 6,000 and 60,000 metric tons of CO2 just from the downloads, before any of the AI actually runs. Google has not publicly responded. [VERIFY THIS]

---

### TAKEAWAY — One clear thing to do or remember

*[Return to screen recording.]*

Here's how to check if this file is on your machine right now.

**On a Mac:** Open Finder. Press Command+Shift+G. Paste this exact path: `~/Library/Application Support/Google/Chrome` — then look inside for a folder called `OptGuideOnDeviceModel`. If you see `weights.bin` inside it, that's the model.

**On Windows:** Navigate to `C:\Users\[your username]\AppData\Local\Google\Chrome\User Data` and look for the same folder name. [VERIFY THIS — confirm paths on current Chrome versions]

If you find it and want to try turning off the features, go to `chrome://flags` in your address bar and search for Gemini Nano. Turning off those flags may reduce what the model does, though whether it prevents Chrome from re-downloading the file afterward is unclear. [VERIFY THIS]

The real decision is simpler than all the technical details: now you know this is there. What you do with Chrome going forward — whether you keep using it, investigate the flags, or look at alternatives like Firefox — that's yours to decide. I'm not telling you to panic or to switch. I'm telling you what's on your computer, because you have a right to know that.

*[End on that. No subscribe prompt. No "let me know in the comments." Just the close.]*

---

**[VERIFY THIS] flags in this script:**
1. Confirm Summarizer API is genuinely callable by third-party sites — find a real implementation example
2. Confirm Hanff filed a formal regulatory complaint (vs. publishing a post/open letter)
3. Confirm Google has issued no public response as of recording date
4. Confirm folder paths for both Mac and Windows on the current Chrome stable release
5. Confirm whether disabling Chrome flags prevents re-download or only disables features

---
*Outline word count: ~750 words*
