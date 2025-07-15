# 🧠 Signal Boost – Morning Tweet Prompt

## What this prompt generates

Produces a **short, morning tweet** designed to gently jolt users out of analysis paralysis, creative fog, or productivity guilt. It uses a randomly drawn perspective card from `cards.json` and leans into Rob’s sardonic, anti-hustle tone. Think: tactical wisdom + cosmic sarcasm to start the day right.

## Format & Tone

* Opens with: `🧠 Signal Boost: [Card Name] [Emoji]`
* One short insight (1–2 sentences), inspired by the card meaning (or reversed meaning 50% of the time)
* Ends with **a bolded self-reflection question**
* Written in Rob’s voice: clever, grounded, irreverent, and never hustle-preachy
* Should feel helpful and witty—not motivational or fluffy
* Entire tweet must fit under 280 characters
* Includes one-sentence `illustration_prompt` for retro anime / Ghibli–style art

## Rules

* Pull a random card from `cards.json` unless a specific one is requested
* 50% chance of using the card’s reversed meaning
* Use the card's concept as a lens for the insight (not a literal description)
* Do **not** explain the card—apply its metaphor to real-world creative stuckness
* Avoid repeating language from the card’s prompt list verbatim
* Optionally, tailor the message toward a target persona using `customer-personas.md`

## Output format

```json
{
  "tweet": "[complete tweet under 280 characters]",
  "illustration_prompt": "[single-sentence retro anime-style prompt]"
}
```

## Example Output

```json
{
  "tweet": "🧠 Signal Boost: Monitor Setup 🖥️ You’re not stuck—you’re just zoomed in too far. Try a side-by-side view of your doubt *and* your progress. **What would change if you looked at the whole screen?**",
  "illustration_prompt": "Retro anime illustration of a dual-monitor setup—one screen shows chaotic notes, the other a focused plan. A floating rubber duck in a wizard hat adjusts the monitor tilt."
}
```

## Don’ts

* Don’t use generic productivity slogans
* Don’t over-describe the card
* Don’t exceed tweet length
* Don’t default to “you got this” or “believe in yourself” tones
