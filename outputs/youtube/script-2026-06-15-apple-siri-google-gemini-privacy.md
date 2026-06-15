# YOUTUBE SCRIPT OUTLINE — 2026-06-15
## Topic: Apple rebuilds Siri on Google Gemini — privacy implications

---

**Title variant A (curiosity gap):** Apple Said Privacy Was Non-Negotiable. Then They Hired Google.

**Title variant B (direct):** Siri Is Now Powered by Google. Here's What That Actually Means.

**Estimated runtime:** ~750 words at natural narration pace (~130 wpm) ≈ **5 minutes 45 seconds**

---

## SCRIPT OUTLINE

---

### HOOK — First 15 seconds

Apple has been saying "privacy in AI is nonnegotiable" for two years.

Last week they announced that some of what you ask Siri will now be processed by Google.

On Google's servers.

Those two things are in direct conflict. Let's talk about it.

---

### SETUP — The problem stated plainly

WWDC was last week — Apple's annual developer conference. The headline was a completely rebuilt Siri. It can handle multi-step tasks, maintain context across a conversation, and take action across your apps. Apple is calling it Siri AI.

It's genuinely more capable than the old Siri. The old Siri was famously terrible. This one is not.

Here's the part that got less attention: Siri AI runs on three different layers. And the third layer is Google.

---

### EXPLANATION — What's actually happening

Apple calls this a tiered architecture.

Simple requests — set a timer, play a song, check the weather — stay on your iPhone. Apple's own smaller models handle those. This part is real, not just marketing.

Moderate requests go to Apple's Private Cloud Compute servers. This is Apple's own cloud infrastructure, designed with stronger privacy constraints than typical cloud services.

Complex requests — ones that need real reasoning, cross-app context, long conversations, nuanced questions — get routed to Google Cloud, where they're processed by Gemini, Google's most capable model. [VERIFY THIS — confirm the three-tier routing architecture from Apple's WWDC technical session before recording]

Apple and Google issued a joint statement that this maintains Apple's "privacy standards." Craig Federighi said "privacy in AI is nonnegotiable" at the keynote. These statements are carefully worded. They ask you to trust both companies simultaneously about what happens at that third tier.

What does Google actually see? What does Google keep? Can Google use those queries for anything — model improvement, debugging, logging? Apple says no. There is no independent audit of Google's end of this arrangement yet. [VERIFY THIS — what does the Apple-Google data agreement actually say about retention?]

---

### NUANCE — The thing most explainer videos skip

Here's what almost nobody is saying: this was a business decision, not a privacy decision. The privacy language came after.

Apple has been behind on AI capability for years. Building a language model as powerful as Gemini in-house would take years and billions of dollars Apple decided not to spend. Using Gemini solves the capability gap immediately. "Privacy in AI is nonnegotiable" was said by the same person who just signed the deal with Google.

That's not necessarily wrong. It's a tradeoff. But it should be understood as a tradeoff, not as Apple solving the privacy problem of AI.

Here's what else most videos skip: whether this matters to you depends entirely on who you already are online.

If you use Gmail, Google Maps, Google Docs, or Google Search — Google already knows a significant amount about you. Adding some Siri queries on top doesn't dramatically change your exposure. You're already inside Google's data ecosystem.

But if you chose iPhone specifically because you wanted to keep Google out — you use Apple Maps, iCloud Mail, DuckDuckGo — this update changes that calculation. You've been paying for that separation. Now some of Siri's most useful new features route through the company you were avoiding.

[YOUR TAKE ON THIS — is this a betrayal, a pragmatic tradeoff, or something in between? What's your honest read?]

---

### TAKEAWAY — One thing to remember or do

The new Siri AI arrives with iOS 27 this fall — iPhone 15 Pro or newer, any iPhone 16. You have time before it lands.

Here's the one thing to carry out of this video:

Apple made a tradeoff. You get a genuinely more capable Siri. In exchange, the most capable features route through Google. That might be fine with you — but it's a choice you deserve to understand before it's on your phone.

**What to watch for:**
When iOS 27 developer betas ship, look for whether there's any user-facing control over routing — a way to limit yourself to on-device processing, even at the cost of some features. If that control exists, it's important. If it doesn't, the choice is all-or-nothing.

And check Apple's WWDC technical session on Siri AI — that's where the architecture details live. Link in the description. [SOURCE NEEDED — specific WWDC 2026 session title]

---

### CLOSING

Privacy promises from tech companies are worth paying attention to. They're also worth reading carefully.

"Privacy in AI is nonnegotiable" turned out to mean: privacy in AI is nonnegotiable, except when we need Google to make it work.

That's still something. It's just not what it sounded like at the keynote.

---

*Notes for recording:*
- The HOOK works best delivered flat and deadpan — resist the urge to editorialize in the first 15 seconds
- The three-tier architecture may benefit from a simple on-screen graphic (phone → Apple cloud → Google cloud) to make it concrete
- Resolve all [VERIFY THIS] flags before recording — especially the Google data retention question
- [YOUR TAKE ON THIS] is the heart of the NUANCE section — don't skip it or soften it
