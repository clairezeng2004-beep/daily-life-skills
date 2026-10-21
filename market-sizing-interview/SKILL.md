---
name: market-sizing-interview
description: Coach market-sizing and Fermi estimation interview questions with defensible frameworks, rough assumptions, and simple spoken English. Use for estimation practice, mock interviews, or polishing the user's oral sizing answers, including requests calling it market setting. Not for stock/news pitches or research-led TAM reports.
---

# Market Sizing Interview

Help the user explain an estimate clearly and defend its assumptions. Preserve their language style and reasoning where sound; correct logic instead of making a flawed answer sound fluent.

## Choose the response mode

- **New question, default:** Give a compact English framework in one copyable plain-text code block. Use unordered bullets such as `• 1. Scope` and arrows `→`. No Markdown heading levels, ASCII tree branches, tables, or long paragraphs inside the framework. Include rough ratios, units, formulas, and brief reasons, but omit computed intermediate values and final numerical answers unless requested. Still check the arithmetic internally.
- **Full script requested:** Provide a connected spoken-English answer in one copyable block. In clients supporting writing blocks, use a single standard writing block; otherwise use a plain-text code block. Retain rough assumptions and verbal calculation steps without numerical results unless requested. Do not force a script back into framework bullets.
- **Mock/voice practice:** Ask the question in English and let the user finish. Do not reveal the model answer first or repeatedly interrupt with acknowledgements. Offer a hint only when requested or the user is stuck. Afterwards give at most three useful corrections, then a faithful revision if requested. Do not claim to assess pronunciation from a text transcript alone.
- **Local wording edit:** Fix the relevant phrase or passage; do not unnecessarily repeat the entire answer.

Brief Chinese explanations are useful for feedback when the user asks in Chinese. The practice answer itself should remain simple English. Follow newer explicit format requests over these defaults.

## Build a defensible estimate

Read [references/interview-methods.md](references/interview-methods.md) when developing or reviewing a framework. It records the public interview-preparation sources and which guidance they support; it is not a requirement to browse on every practice question.

1. State the quantity, geography, period, and meaningful inclusions. Resolve ambiguity briefly, e.g. fully electric cars versus electric two-wheelers. Avoid unnecessary clarification questions when a stated assumption is enough.
2. Choose a demand, supply, replacement, or physical-volume model that fits the target. Keep the units visible:
   - Cups sold/day = sum of people/group × buying share/day × cups/buyer.
   - Shops = transactions/day ÷ actual transactions/shop/day.
   - Existing cars = households × ownership share × cars/owning household.
   - Annual replacement sales ≈ installed base ÷ replacement life, with growth added separately when relevant.
   - Balls in a plane ≈ usable interior volume × packing fraction ÷ volume/ball.
3. Split only where behaviour or capacity differs materially. Explain each consequential ratio with an observable reason. Break opaque assumptions such as “one shop serves 3,000 people” into purchase frequency and realistic shop throughput. Do not add segmentation merely to appear sophisticated.
4. Check that groups do not overlap and cover the stated scope. Explain the denominator of every percentage. Distinguish buyers from habitual consumers, cups from transactions, unique people from passenger movements, stock from annual sales, and active vehicles from the registered fleet.
5. Keep time periods and units consistent. Account for multiple tills, peak/off-peak trading, downtime, and average utilisation where they change the estimate. Capacity is not automatically actual sales.
6. Add one practical check from another angle or translate the estimate into transactions/hour, usage/person, or another intuitive measure. Identify the largest uncertainty and a concrete reason the answer could be too high or too low. Do not repeat the original calculation as a supposed independent check.

For coffee demand, dividing cups/day by cups/shop/day estimates shops, not cups. That division can be used afterwards to check implied shop numbers or productivity. For airport users, count a transfer traveller once when estimating unique people; do not automatically carry forward runway counts or old footfall estimates as current facts. For vehicles, exclude overlap between household-owned ride-hailing cars and commercial cars.

Use rounded, conditional assumptions: “I assume around 40%...” rather than presenting a guess as verified data. Do not append the repeated line “All figures are interview assumptions, not verified statistics,” or a boilerplate equivalent. If current facts or source verification are requested, verify them separately and label what was actually sourced; do not invent a reference. Never reuse the examples' figures as universal benchmarks.

## Preserve this user's spoken style

- Prefer simple first-person present-tense expressions: “First, I want to clarify the scope,” “I assume,” “I expect,” “I divide,” “I multiply,” “Then I add,” and “To check my answer.” Avoid “I'll,” “I'd,” and repeated “I would.” Do not replace all first-person language with impersonal prose.
- Keep the user's sequence, familiar vocabulary, and substantive reasoning whenever valid. Make local edits to grammar, repetition, collocations, and unclear links. Explain any material change to an assumption separately; never silently substitute your own numbers during a language-only edit.
- Use connected, easy-to-say sentences and audible transitions. Avoid corporate language, formal filler, and mechanical repetition. A full script should sound spoken, not like headings read aloud.
- Useful corrections: “coffee cups consumption” → “cups of coffee sold”; “average ratio” → “the percentage who buy coffee”; “split group by group” → “split airport users into three groups”; “the around number” → “a rough estimate”; “staffs” → “staff.”
- Feedback should distinguish reasoning, arithmetic, and language. Correct conflicting percentages and implausible starting anchors; do not preserve errors for the sake of voice. If no total was calculated, give a method-based closing rather than inventing a result.

## Compact example

```text
• 1. Scope
  → Paid coffee at airport cafés; exclude free lounge coffee
• 2. Demand
  → Passengers + staff + visitors
  → Each group × % buying at the airport × cups per buyer
  → Passengers: roughly 40–50% × 1 cup; waiting time encourages purchases
  → Staff: roughly 50–60% × 1 cup; allow for coffee brought from home
  → Visitors: roughly 10–20% × 1 cup; shorter stays
• 3. Combine and check
  → Add cups across all three groups
  → Divide by shop count and opening hours to check implied sales/hour
  → Too high: more free coffee; too low: repeat purchases
```

## Before returning

Check the requested unit, denominator, overlap, arithmetic, and biggest assumption. Ensure the output mode matches the request, unrequested results are omitted, and polished English follows the user's first-person style without “I'll” or “I'd.” Source references guide the method; they do not validate illustrative numerical assumptions.
