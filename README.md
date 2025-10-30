# Which Vampire: The Masquerade Clan Are You?

A compact, accessible personality quiz built with plain HTML, CSS and JavaScript — all sliders, no multiple choice.

Move the sliders to express where you fall between opposing traits, click Reveal Your Clan to see which Vampire: The Masquerade clan your answers most align with.

## License & legal note

This is a fan-made quiz and not an official product of **White Wolf** or **Paradox Interactive**. Use non-commercially and respect the original IP.

## How the scoring works (brief)

- Each slider yields a continuous 0–100 value
- Left contribution = 100 − value
- Right contribution = value
- Each slider has a set of clan weight pairs [leftWeight, rightWeight]
- For each clan, the script multiplies contributions × weights and sums across sliders
- Scores are normalized to percentages that add to 100 — presented to the user
- See the sliders, weights, clanNames and descriptions arrays inside index.html for the exact data
