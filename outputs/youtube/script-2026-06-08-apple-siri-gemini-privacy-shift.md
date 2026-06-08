# YouTube Script Outline — 2026-06-08
**Topic:** Apple WWDC / Siri + Gemini privacy shift
**Slug:** apple-siri-gemini-privacy-shift

---

**Title A (curiosity gap):** "Apple just handed Siri to Google. Here's what it actually means."
**Title B (direct):** "Siri is now powered by Google Gemini — Apple's privacy promise, explained"
**Estimated runtime:** ~5.5 minutes at natural narration pace (~130 wpm / ~720 words of spoken content)

---

## HOOK — first 15 seconds

Apple has had one brand promise that's outlasted every product cycle: your data stays with you. Today, at their developer conference, they announced Siri will be powered by Google. That's a sentence worth pausing on.

---

## SETUP — the problem stated plainly

Apple WWDC is where Apple announces the features coming to your iPhone, iPad, and Mac later in the year. Today — June 8, 2026 — they unveiled the biggest Siri overhaul in years.

New chat mode. Conversational. Multi-step. Can handle context across a whole session. And a feature called "personal context" — if you opt in, Siri can read your calendar, your messages, and your email to give more useful answers.

And for queries that Apple's own AI models can't handle: Google Gemini.

That last part is the one worth talking about.

---

## EXPLANATION — what's actually happening

Apple's AI system already had two layers before today. The first layer is on-device processing — small models running locally on your iPhone, handling simple tasks without anything leaving your device. The second is something called Private Cloud Compute — Apple's own cloud infrastructure, designed with specific privacy architecture.

Apple has published detailed documentation on Private Cloud Compute. Privacy researchers have audited it. The commitments include: Apple employees can't access your data, data isn't retained after the request completes, and it can't be used to train new models. [VERIFY THIS — confirm current PCC commitments as of WWDC 2026] That's a meaningfully different set of promises than what most cloud AI services offer.

Today adds a third layer. Some queries go to Google. Not to Apple's architecture with Apple's commitments. To Google.

Google's business model is built on understanding user behavior. That's not a criticism — it's a description of how they've built one of the most valuable companies in history. But it means that when your Siri query lands on Google's infrastructure, you're under Google's privacy policy, not Apple's.

---

## NUANCE — what most coverage will miss

Here's the nuance that will get lost today, because most headlines will be about "Apple uses Google."

Apple was already routing some AI queries off your device — just to Apple's own systems. So this isn't a new privacy category. What it is: an escalation. Instead of Apple's cloud with Apple's commitments, some queries now go to a third party.

The piece that's not yet clear is what happens with "personal context." If you opt in to giving Siri access to your calendar and messages, and Siri routes a query to Gemini — what does Google receive? Just the abstract question? Or the personal context that shaped it? [VERIFY THIS — Apple has not fully documented this in the WWDC announcement] That's the specific question to watch for in Apple's technical documentation over the coming weeks.

There's something else worth noting. Apple is also opening its AI framework so that developers can choose which AI model powers their app — Apple's models, OpenAI, Anthropic, or Gemini. This means that the AI assistant inside any given iOS app could be sending your data to any of those providers, and you'll likely never see a prompt about which one. Apple's privacy story is now fragmented across every app that builds on this system.

---

## TAKEAWAY — one clear thing to remember

These features won't ship until iOS 27 in the fall. [VERIFY THIS — confirm release timeline] That window is useful. Before you update and enable personal context, wait for the technical documentation — not the keynote summary, the actual documentation. Privacy researchers and organizations like the EFF will analyze it. That analysis is worth reading before you opt in to anything.

If you use Siri for sensitive conversations — health, legal, financial — that's the category to be most cautious about until the data flows are clearly documented.

The thing to carry with you: Apple may still be the most privacy-careful company in your daily tech life. That's not the same as saying this is fine. "More protective than the alternatives" has been doing a lot of work in Apple's privacy marketing. Today makes that work a little harder to do quietly.

---

*Production notes: Consider showing the WWDC stage + the privacy billboard side by side. Avoid taking a "Apple lied" tone — keep it measured and specific. The story is about what we don't know yet, not a clear betrayal.*
