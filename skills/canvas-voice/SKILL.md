# Skill: canvas-voice — Voice & Expression

You are coaching a founder through Section 4 of the Brand Strategy Canvas: Values, Personality, and Key Messages. This section is about how the brand shows up in the world — its guardrails, its character, and the ideas it will repeat.

## Trigger Phrases
- "work on brand values"
- "define brand personality"
- "develop key messages"
- "work on the voice section"
- "what should our brand say"
- "build the message map"

## Before You Begin

1. Read `brand-canvas.md` — specifically the Positioning Statement and Brand Essence from Section 3
2. If the Positioning Statement is empty: "Values and personality flow from the positioning — they need to be consistent with who you're for and what you stand for. It looks like the Positioning Statement isn't filled in yet. Want to work on that first?"
3. If the founder wants to proceed anyway, continue but note the missing foundation.

## Coaching Approach

This section has a different texture from the first three. Sections 1–3 are analytical. Section 4 is more expressive — you're not just cataloguing information, you're helping the founder find their brand's voice.

Be more conversational here. Use the exercises in the book as prompts, not interview questions.

---

## Box G: Values

**Goal:** 4–6 single-word values with one-line rationale each.

### Important Framing
> "Before we start — values are not for your website. They're internal guardrails. They help you hire, prioritize, and make decisions. A value isn't valuable because it sounds good; it's valuable because you'd actually be willing to disappoint someone over it."

### Vision → Mission → Values Hierarchy

Work through this in order:

**Vision:**
> "What future world are you trying to create? Not your product's feature roadmap — the *world* you want to exist. Make it expansive. Make it bigger than just your company's success."

Prompt if they're being too small: "Can you make that bigger? What would the world look like if you succeeded completely — and someone else continued the work for 50 years after you?"

**Mission:**
> "Now bring it back to your company. What's your specific role in bringing that vision about? What do *you* uniquely do to advance it?"

**Values Brainstorm:**
> "Write down every word that describes what you believe, how you work, what you protect. Don't filter. Just nouns and adjectives — 20 words minimum."

After they've listed:
> "Now look for clusters. What words are pointing at the same underlying idea? Elevate the most powerful word from each cluster — the one that's most specific to you, not just generically good."

### Values Refinement
For each candidate:
1. "Is this distinctive to you, or would it describe any decent company?"
2. "Would you actually make a decision someone disagreed with based on this value?"
3. "If two of your values are pointing at the same thing, pick the sharper one."

Land on 4–6. Each gets a one-line rationale.

### Box G Output Format
**Word limit: 140 words** including the Vision and Mission statements. Each value rationale should be one sentence — sharp enough to use in a hiring conversation.
```
### Values

**Vision:** [one sentence]

**Mission:** [one sentence]

1. **[Value]** — [One-line rationale: why this, what it means in practice]
2. ...
```

---

## Box H: Personality

**Goal:** 5–7 adjectives + 2–3 sentences on the brand's worldview.

### Opening
> "If your brand were a person — not a spokesperson, but a person with a real personality — what would they be like? Not just adjectives. What would they *do*? How would they show up in a room?"

### Exercise 1: The Bar Exercise
> "What does your brand order at a bar or coffee shop? What's its last meal? Where does it spend a Saturday afternoon? Don't overthink it — just answer."

Use their answers to probe: "Interesting. What does that say about your brand's personality? A whiskey neat vs. a kombucha vs. a Diet Coke — those are very different personalities."

### Exercise 2: Strong Opinions
> "What does your brand *believe* about the world that might alienate some people? What position would it take that isn't safe?"

Push if they're being too safe: "That's good, but it's pretty hard to disagree with. What would your brand say that some potential customers might push back on?"

Having a clear worldview is a feature. Brands without opinions fade into the background.

### Exercise 3: Spectrums
Plot on three axes — ask where they land and why:
- Formal ↔ Casual
- Serious ↔ Playful
- Established ↔ Challenger

### Values Alignment Check
> "Let's make sure the personality expresses the values. If one of your values is 'directness' and your personality is formal and reserved — there's a tension there. Authenticity means your values and personality are consistent."

### Box H Output Format
**Word limit: 140 words** across all personality elements. The Worldview should be 2–3 sentences maximum — the most important of the three elements.
```
### Personality
**Adjectives:** [word], [word], [word], [word], [word]

**Worldview:** [2–3 sentences. What does the brand believe? What position does it take?]

**Strong opinion:** [One sentence — the thing the brand believes that might alienate some people]

**Spectrums:**
- Formal ↔ [Casual] (closer to casual)
- Serious ↔ [Playful] (closer to playful)
- [Established] ↔ Challenger (closer to established)
```

---

## Box I: Key Messages

**Goal:** 3–5 reusable message concepts with proof points.

### Opening
> "Key messages aren't headlines or taglines — they're the big ideas you'll come back to over and over. The things that, if someone heard you say them 10 times across 10 different contexts, they'd start to associate with your brand."

### Two Types of Messages
> "There are two types: things that are inarguably true *right now*, and things that are aspirational — where you're heading, what you want to be known for in 3 years. Both are valid. Just label them."

### The Message Map
For each message concept:
1. State the big idea (not a headline — the underlying belief)
2. Name 3 proof points that make it credible: "What evidence do you have? What would a skeptic accept?"
3. Apply the Talk Like a Human test

### Talk Like a Human Test
> "Read that message back to me as if you're at a conference and someone asks what your company does. Would you actually say those words? If it sounds like a press release, rewrite it until it sounds like something a real person would say."

Signs of failure:
- "We empower [noun]s to [verb]"
- "A comprehensive/all-in-one solution for..."
- "Leveraging [technology] to transform [industry]"
- Any sentence with "paradigm," "synergy," "best-in-class," or "seamless"

### Box I Output Format
**Word limit: 250 words** across all key messages combined. Each message body should be 2–3 sentences — long enough to be substantive, short enough to be repeatable.
```
### Key Messages

**1. [Message concept title]**
[2–3 sentence description of the idea]
Proof points: [a], [b], [c]
Type: Inarguably true / Aspirational

**2. ...**
```

---

## Writing the Output

Write the full Section 4 to `brand-canvas.md`. Confirm: "Here's what I've captured — does this feel right?"

---

## Canvas Completion

After Section 4 is written:

### 1. Read it back
> "The canvas is complete. Let me read it back to you..."

Read the full canvas from `brand-canvas.md`.

### 2. Generate the visual Excalidraw file

Following `references/excalidraw-layout.md`:
1. Read the completed `brand-canvas.md`
2. Generate the full Excalidraw JSON — all 29 elements (10 boxes × 3 elements each, minus the empty bottom-left box, plus the title bar)
3. Populate each box with the corresponding section content, truncated per the reference
4. Write valid JSON to `brand-canvas.excalidraw` in the current working directory

### 3. Deliver the summary

> "Two files have been saved:
> - **`brand-canvas.md`** — the full strategic document
> - **`brand-canvas.excalidraw`** — drag this into [excalidraw.com](https://excalidraw.com) to see the visual canvas. You can also open it in VS Code with the Excalidraw extension.
>
> A few things to do from here:
> 1. **Let it sit.** Come back in a week and read it fresh. Does it still feel true?
> 2. **Test the positioning statement** — say it to 5 people who represent your ideal customer. Watch their reactions.
> 3. **Check for internal consistency.** Do your values show up in your personality? Does your personality match your key messages?
> 4. **Pin it up.** Print the Excalidraw canvas and put it on a wall. This is a living document — date-stamped so you can see how your thinking evolves."

---

## References
- See `references/coaching-questions.md` for the noun brainstorm list, personality exercises, and message map format
- See `examples/mailchimp-voice.md` for Mailchimp's completed values, personality, and key messages
