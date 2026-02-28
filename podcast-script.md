# Podcast Script Generation Prompt

## Purpose
This prompt generates a conversational podcast script from source material (study guides, notes, articles). Use this when you want to manually create a podcast-style script — for example, to review as a dialogue, use with a TTS tool, or when you don't have access to Google NotebookLM's auto-generated Audio Overview.

If you **do** have NotebookLM access, you may not need this prompt — just upload your study guide (see `study-guide.md`) and use NotebookLM's built-in podcast generation. This prompt is for manual/custom control over the script.

## Prompt

---

Transform the following source material into a podcast script — a conversational deep-dive between two hosts.

**Source material:**
[PASTE STUDY GUIDE OR NOTES HERE]

### Host Personas
- **Host A** ("The Expert"): Has deeply studied the material. Drives the narrative, explains concepts clearly, and shares the key insights. Confident but not condescending.
- **Host B** ("The Sharp Learner"): Smart and curious — not a beginner, but encountering this specific topic fresh. Asks clarifying questions, makes analogies to familiar concepts, pushes back when something sounds too simple, and reacts naturally ("Wait, that's wild" / "OK so basically..." / "Hold on, let me make sure I get this").

### Guidelines
- **Duration**: ~15-20 minutes of spoken content (~3,000-4,000 words)
- **Tone**: Energetic and natural — two smart people geeking out over a topic, not reading a textbook
- **No filler**: Every exchange should teach something or build understanding. Cut "great question!" padding.
- Host B should interrupt naturally — real conversations aren't turn-by-turn monologues
- Use **concrete examples and analogies** — at least 3-5 throughout
- Build complexity gradually — start accessible, earn the nuance
- Include at least one "the thing most people get wrong" moment
- Include at least one "OK this is the part that blew my mind" moment
- End with a clear, memorable takeaway

### Script Format

```
[Host A]: dialogue here

[Host B]: dialogue here
```

### Structure
1. **Cold open** (~30 sec) — Hook the listener. Why should they care about this right now?
2. **Level set** (~3-4 min) — Core concepts explained simply. Get everyone on the same page.
3. **The deep dive** (~8-10 min) — Nuances, trade-offs, real examples, the interesting stuff. This is the meat.
4. **The twist** (~2-3 min) — A common misconception, a surprising insight, or a counterintuitive finding. The "aha" moment.
5. **So what?** (~2 min) — Practical takeaway. What should the listener do with this knowledge?
6. **Wrap** (~30 sec) — Quick recap of the 2-3 things to remember.

### Quality Checks
- Would this sound natural if read aloud? (No walls of text in a single turn)
- Does Host B actually add value, or are they just saying "wow, interesting"?
- Are there enough concrete examples that a listener could retell them?
- Is the complexity curve right — simple start, satisfying depth, clear landing?

---

## Usage

1. First generate a study guide using `study-guide.md` prompt
2. Paste the study guide as source material in this prompt
3. The output script can be:
   - Read as a dialogue for personal review
   - Fed to TTS services for audio generation
   - Used as a planning doc for actual recording
