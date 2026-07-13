# SUPERGROUP — one-page design (v0.1)

*Draft the greatest band ever assembled. Beat the House.*

## Thesis
Immaculate Grid / 82-0 proved that **luck + skill + competition + a shareable score** is a viral engine.
Every hit in that genre lives on **male-skewing sports trivia**. SUPERGROUP points the same loop at
**music knowledge** — broader, more gender-balanced, funnier to share ("look at the band I made").

## Core loop (≈60 seconds)
1. You draft a 5-piece band, one role at a time: **🎤 Vocals · 🎸 Guitar · 🎻 Bass · 🥁 Drums · 🎛️ Producer**.
2. Each role deals you a **slot machine of 3 candidates** (name + genre shown, **power rating hidden**).
   You pick with your gut and your knowledge. **2 rerolls** per game (the 82-0 "skip").
3. The **House** silently drafts its own band from the same pool (greedy: always grabs the biggest name).
4. **Reveal:** every card flips to show its **Legend Rating** + a real credential. Sum your band,
   add **Chemistry** bonus, compare to the House. Win or lose.
5. **Share** a link — your friend replays the *exact same seed* (same House, same deals) to beat your score.

## Why it's addictive
- **Knowledge is the edge:** ratings are hidden at pick-time, so you must *know* that McCartney (bass!) or
  Quincy Jones is a monster value. Casual players survive on recognition; heads win on depth.
- **Luck is real:** the deal decides what's on offer. Bad deal? Spend a reroll — or gamble.
- **Chemistry rewards taste:** stack 3+ of one genre for a bonus, so the biggest name isn't always right.
  This is the skill layer that beats the House (which never plays for chemistry).
- **The House first, friends second** (the 82-0 insight): always-on single-player, no dependency on a friend
  being online. Head-to-head is the *same engine* with a shared seed link.

## Scoring
- Band score = Σ Legend Rating (0–100 each) of your 5 picks **+ Chemistry** (3 same genre +12, 4 +25, 5 +40).
- Ratings are a **curated ground truth** (internally consistent, balanced for play), each **anchored to a
  real credential** on reveal so it reads as fair and teaches something.

## Tech / constraints
- Single self-contained `index.html`, vanilla JS, mobile-first portrait. No build, no backend, no accounts.
- **Seeded PRNG** → the whole game is reproducible from a URL seed, which is what makes the share loop work.
- Deploy: GitHub Pages → a URL you text to a phone.

## Roadmap (post-hour)
- v2: head-to-head pass-and-play & async challenge scoreboard; daily seed; "build-a-cast" movie variant;
  bigger/curated dataset with sourced stats; genre-locked themed decks (80s, Hip-Hop, Divas).
