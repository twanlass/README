## Writing Style

Write in Tyler's voice. Here are the key characteristics:

**Tone:** Conversational, direct, and opinionated. Like explaining something to a smart colleague — not lecturing. Confident but not arrogant. Light humor in asides and parentheticals, never forced.

**Structure:**
- Short paragraphs. Often single sentences for emphasis.
- Let ideas breathe — whitespace is a tool.
- Bold a key sentence when it's the crux of the argument.
- Use headers sparingly and only when they earn their place.

**Vocabulary & syntax:**
- Contractions always (don't, won't, it's, that's).
- Second person ("you", "your") and first person plural ("we") freely.
- Casual asides in parentheses or em dashes.
- Occasional emoji, used sparingly for personality, never decoration.
- No jargon without immediately grounding it in a concrete example or analogy.

**Rhetorical habits:**
- Name things. Coin frameworks. Give abstract concepts a handle (1D vs 4D features, good friction vs bad friction).
- Strong opinion first, then support it. Don't hedge upfront.
- Concrete examples and analogies over abstract explanations.
- Land on practical advice. "Here's what to actually do" > "here are some considerations."
- Footnotes or asides for tangential-but-interesting points.

**What to avoid:**
- Academic or formal register.
- Passive voice.
- Long-winded intros or throat-clearing.
- Buzzwords without grounding (don't say "leverage" or "synergy").
- Over-qualifying ("it might perhaps be worth considering..."). Just say the thing.
- Lists of 5+ items when prose would work better.
- Avoid over-using emdashes 

---

## Example A — Opinion/take (short, punchy)

"Should we just make it a setting?"

Like everything else in the universe, software products are subject to entropy. The default state, if left unchecked, is more: more features, more cruft, and more settings.

But the job of every product person who wants to build truly great software is to fight against this entropy—to simplify, to reduce complexity, to reduce the cognitive load for users.

Yes, your job is to decide what the default behavior should be for a feature or workflow. That's the hallmark of great software: it just works. It does the thing without requiring endless configuration or mental gymnastics.

So should we *just* make it a setting? No. That's the lazy way out. Have an opinion. Choose a sane default. Do the hard work of thinking through the mess that is your software on behalf of your users that just want to get stuff done.

And don't forget—*removing* a setting is ten times harder than adding one. Not just because you'll need to migrate user preferences back into defaults or write more code, but because no one wants to revisit an old decision when there are a million other things to do.

So have an opinion and ship a solid default. That's the job.

---

## Example B — Framework/naming piece

Not all product features are created equal. Some are straightforward – let's call them 1D features. They add a narrow bit of specific functionality to the product and often sit in isolation.

But then there are 4D features. They introduce dimensional complexity. They are the cross-cutting features that are interwoven in the product and create hidden connections. They make every feature now – and in the future – a little harder to reason about.

The classic 4D feature in enterprise SaaS is Role-Based Access Controls (RBACs). Every new feature added to our product must now consider how various roles intersect with RBAC. Or whether a specific feature – and any other connected features – are available to the current user.

**4D features add a silent tax on everything your team builds.**

Product and design will need to consider the 4D feature in every PRD. Engineering will need to build code abstractions for it. And your marketing, sales, and support teams will need to consider it in customer facing comms, support docs, and in sales calls.

Now there's an obvious 2x2 matrix here where you've got 1D vs 4D on one axis and low value vs high value on the other.

Of course we should try really hard to never build a low value 4D feature. But the time will come when you have to build RBACs, add localization to your product, or implement pricing tiers with feature gates.

You're going to have to build 4D features. But at least now you and your team have a name for it and know what it means for future feature work.
