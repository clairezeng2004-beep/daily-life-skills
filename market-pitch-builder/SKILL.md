---
name: market-pitch-builder
description: Turn market articles, research reports, or news into evidence-grounded stock pitches and news pitches for Sales and Trading interviews, with a confident first-person voice and clear separation of source evidence from added interpretation.
---

# Market Pitch Builder

Build an interview-ready market view from third-party research without inventing missing evidence. Support stock pitches and news pitches, including long-only, short-only, and explicitly requested relative-value trades. This skill owns investment logic and source fidelity. Use the sibling [video-interview-answer-polisher](../video-interview-answer-polisher/SKILL.md) skill for the final spoken-language polish.

## Establish the requested scope

Use the conversation to identify the company or event, direction, interview context, language, and word limit. Do not ask again for information already supplied.

- Default to natural spoken English for an interview pitch; use the user's requested language otherwise.
- If asked for a long pitch, centre the chosen company. A potential hedge mentioned earlier does not authorize continued long/short framing.
- If the user supplies a screenshot framework, follow its useful structure, treating its examples as examples rather than company facts.
- Keep each final English pitch at or below 250 words, including any headings within the pitch; follow a shorter requested limit when supplied. Put optional research notes, citations, and any requested Chinese explanation outside the pitch. Expand supporting material only when requested.
- Tailor an IED/Sales and Trading pitch toward a clear view, why the price could change, timing, and risk. Do not force bank slogans or a generic role connection into it.

## Read the evidence before drafting

Read the linked report itself, through the signed-in browser when appropriate. Distinguish full-text access from title, summary, or search-snippet access. If access is partial, disclose that briefly and write only what the accessible evidence supports; do not reconstruct an unseen article.

Record publication date, financial period, forecast year, and price date separately. Prefer recent reports when sourcing ideas; give actual publication dates, not merely crawl dates. Refresh current facts when necessary, but respect a request to stay within the supplied report. Put supplementary research in a separate labelled evidence section rather than silently attributing it to that report.

Maintain a compact working claim ledger:

| Proposed claim | Source passage or location | Period / definition | Status |
|---|---|---|---|
| Material claim | Supporting evidence | Relevant date and metric basis | Direct source / interpretation / missing |

Use the ledger to preserve these distinctions:

- Historical results, management guidance, consensus estimates, and the author's forecasts or opinions are different evidence types.
- Buy, Hold, Sell, profit-taking, and an explicit short recommendation are different conclusions. Do not upgrade Hold or profit-taking into an established short thesis.
- A suggested catalyst is not an announced event. A forthcoming earnings release is not automatically a source-backed catalyst or a reason for a positive reaction.
- Specify GAAP versus adjusted metrics, group versus segment margins, and the forecast year underlying valuation multiples. Never describe a multiple on earnings several years ahead as ordinary next-year forward P/E.
- Fiscal periods may differ between peers. Explain material misalignment and business-mix differences rather than presenting a precise comparison as fully like-for-like.
- Verify peer relationships before calling companies direct competitors. Product overlap does not prove competition for every customer or project, share gains, or a supplier relationship.
- Report-level judgments such as temporary revenue delay rather than permanent demand loss remain judgments when recast in the candidate's voice.

Do not invent a target price, upside, investment horizon, consensus gap, market share, industry forecast, borrow cost, hedge ratio, downside case, or catalyst. Use specific placeholders such as [forecast-year EPS], [confirmed catalyst/date], or [target multiple] when needed. If the user will supply missing material, proceed with those placeholders instead of asking repeated questions.

## Turn research into a view, not a research plan

Draft in a confident first-person voice: "My stock pick is...", "I recommend...", "I think...", "The main risk is...". Do not repeatedly say "the report says" or "the author believes" inside the spoken pitch unless attribution is requested.

This voice does not claim the candidate conducted interviews, built a model, independently verified data, or authored the original research. Keep source links and evidence notes outside the speech, and paraphrase rather than copying distinctive wording. Respect source quotation and summarization limits.

Avoid making the speech about future diligence: "I would examine", "I would test", "I would focus on", or "I would need to show". Such statements belong in a separate missing-evidence note. Conditional language remains appropriate for genuine scenarios and risk responses.

Make the conclusion explicit before explaining what to monitor. "Diesel matters for inflation" identifies a topic; a view states the expected outcome and why, such as "I expect fuel inflation to remain persistent because shipping and refining capacity cannot recover quickly." Use such a claim only when the evidence supports it, and identify added interpretation outside the speech.

For each main thesis, connect an expected outcome to a concrete causal mechanism and its market implication. Give the relevant horizon, comparison, and invalidating condition where supported. Explain which force is likely to dominate in the base case; avoid ending with symmetrical possibilities such as "inflation could hurt bonds, but weaker growth could help" without a judgment. If the evidence cannot support a direction, narrow the claim or omit that asset instead of manufacturing conviction.

Monitoring points should test an already stated view. "Watch tanker traffic" is not a substitute for predicting whether supply is likely to recover. Likewise, "gold offers diversification" does not by itself express a price view. Explain the expected effect of the event without assuming that a useful hedge must rise or that a favourable business development makes a security cheap. Do not invent mispricing or a consensus disagreement to make the view sound distinctive.

Do not make unsupported certainty sound like conviction. A clear base-case judgment can be expressed directly while retaining the condition that would invalidate it. Remove empty assertions such as "the business doesn't need a major announcement every quarter" unless the source supports a concrete mechanism that matters to the trade.

When asked whether the original author made a claim, answer candidly using the ledger. Identify additions and corrections; do not defend an earlier draft by stretching source meaning.

## Stock pitch structure

Follow a supplied framework. Otherwise use this flexible sequence:

1. **Recommendation and company:** Direction and plain-English business description. Include price, horizon, and upside only when available.
2. **Operating thesis:** Usually two distinct company arguments explaining how business developments affect earnings or cash flow. Add an industry argument only if supported and genuinely distinct.
3. **Catalyst:** A specific event or milestone, its timing when verified, and the mechanism by which it could change expectations or pricing.
4. **Valuation:** Explicit forecast period, metric, multiple, target and return scenarios where supported. Keep valuation out of the operating thesis to avoid repetition; a short opening recommendation may still state target/upside.
5. **Risk and conclusion:** Main risk, what would undermine the view, and a brief restatement of the recommendation. Integrate risk where it sounds most natural.

Do not force three theses when the report contains only two. "AI spending is growing" is industry context unless it establishes a specific company benefit. "This is a good business" and "this stock is attractive at today's price" require different support.

For a single-name pitch, use a competitor only when a brief comparison materially strengthens the argument. Keep the company's own operating drivers central. For an explicitly requested pair, establish the independent short case and explain imperfect hedging; do not assume equal-dollar exposure is market-neutral.

## News pitch structure

Use the following four-part structure:

1. **Factual — what happened:** State the key fact or event directly in one sentence, including timing and what was new where relevant. Avoid openings such as "UBS reported" or "the article says"; keep source attribution outside the spoken pitch unless needed to identify an allegation or disputed claim.
2. **Why it happened:** Default to one short sentence explaining the central underlying cause or disagreement. Name the relevant parties and preserve the causal meaning; avoid a numbered list of causes, extended background, or a retelling of events. Add detail only when essential to understanding the thesis or explicitly requested. Keep most of the pitch for directional market views, their transmission mechanisms, and the event outlook. Distinguish supported drivers from interpretation and do not invent motives.
3. **Thesis — impact across different asset classes:** State a clear directional expectation for the relevant markets, including equities and gold where relevant, and explain each in a short causal chain from the event to supply, demand, costs, or earnings and then to pricing. Separate assets or products when their mechanisms differ. Express a reasoned base case with necessary conditions, without making uncertainty the entire conclusion. A natural spoken transition is: "Next, let me walk you through the impact on different markets."
4. **My view — what happens next:** Predict how the underlying event itself is likely to develop over a stated horizon: for example, escalation versus negotiation, policy implementation, or changes in the parties' behavior. Explain why that path is most likely and what development would change the judgment. Where relevant, assess whether the current market reaction is justified. Keep asset forecasts in Impact; do not repeat them here as the main view.

Separate observed price reactions from expected future reactions. Distinguish announcement date from effective date. Describe a consensus disagreement only if expectations are evidenced. Do not force a trade recommendation into a request for news interpretation alone.

## Spoken style and delivery

Before delivering a final pitch, read and apply [video-interview-answer-polisher](../video-interview-answer-polisher/SKILL.md) from this repository. Use its spoken-language editing and final quality check to make the English clear, natural, and easy to follow on first hearing. Preserve this skill's stock/news pitch structure, market reasoning, source distinctions, and evidence constraints; do not replace them with the polishing skill's default point-support-takeaway structure or behavioral interview framing. Language polish must not add claims or turn a conditional forecast into a fact.

- Write as a thoughtful candidate speaking naturally, with short sentences and concrete causal explanations.
- Avoid repeated "I would", formal essay language, generic enthusiasm, excessive jargon, and strings of three abstract nouns.
- Prefer direct, familiar wording that a listener can understand once. Replace opaque market expressions with a concrete trigger and consequence; for example, "prices could rise sharply if production is disrupted" is clearer than "prices remain vulnerable to upward spikes". Preserve the distinction between a possible spike and a sustained trend.
- Explain unfamiliar sector or market terms briefly in plain language, using a short example only when helpful. Cut low-priority assets or detail before adding jargon or longer explanations.
- Make scope precise: name the institution or country providing support, distinguish loans from grants and approved funding from disbursements, and do not equate financial aid with supplier orders. Keep established facts separate from forecasts about future support.
- Use numbers selectively; each should strengthen the argument and be explainable if challenged.
- Count the words after polishing and revise until the final English pitch is no more than 250 words. Cut weaker points and repetition rather than compressing the answer into dense sentences. Do not promise an exact speaking duration.
- Keep citations outside the reusable speech. Where writing blocks are supported, place only the pitch itself in one block.
- For a final-draft-only request, return the speech with at most a brief note about remaining placeholders. Do not append a research checklist or unsolicited long/short discussion.

Before delivering, check that every material claim is supported or visibly conditional, valuation years are clear, thesis points do not duplicate valuation, and the catalyst is not fabricated. A listener should be able to state what outcome the speaker expects, why it is more likely than the main alternative, and what would invalidate it. Revise any passage that only lists important variables, explains generic asset behaviour, or proposes future research without communicating a view.
