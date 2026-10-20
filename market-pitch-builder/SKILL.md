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

For policy-event pitches, verify the relevant year's meeting calendar before explaining the month of a forecast. Distinguish the next scheduled opportunity from a prediction of action; a meeting date alone does not support a hike or cut forecast. Do not imply that action outside scheduled meetings is impossible.

Do not jump from an event forecast to a trade recommendation. Explain what may already be priced in, what would change expectations, and how that change affects the named asset. For rates, distinguish delaying a hike from reducing the total expected tightening; a delay alone may have little price impact. Name the relevant maturity when it matters, and omit the trade if evidence does not support the link.

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

Use three visible section labels in this order, with a colon after each: `Fact:`, `My view:`, `Impact:`. Place each label at the start of its section in the returned English pitch. Keep these labels inside the pitch's word count. Follow a different format only when the user requests one.

1. **Fact:** State the key event directly in one sentence, including timing and what was new where relevant. Add at most one short sentence explaining the central underlying cause or disagreement when needed. Name the relevant parties, distinguish supported drivers from interpretation, and avoid extended background or invented motives. Keep source attribution outside the spoken pitch unless needed to identify an allegation or disputed claim.
2. **My view:** State a clear judgment about the event or its main economic consequence over a relevant horizon. Explain the supporting reasons with brief spoken numbering where useful. For an event outlook, explain the most likely path and what would change that judgment. Avoid repeating the factual setup or replacing a view with monitoring points.
3. **Impact:** Translate the view into directional expectations and client positioning across relevant asset classes. Explain each through a short causal chain from the event to supply, demand, costs, or earnings and then to pricing. Separate assets or products with different mechanisms. Include equities and gold where relevant, and identify the main risk to the call. Keep most of the pitch for the view and its market implications.

Separate observed price reactions from expected future reactions. Distinguish announcement date from effective date. Describe a consensus disagreement only if expectations are evidenced. Do not force a trade recommendation into a request for news interpretation alone.

## Spoken style and delivery

Before delivering a final pitch, read and apply [video-interview-answer-polisher](../video-interview-answer-polisher/SKILL.md) from this repository. Use its spoken-language editing and final quality check to make the English clear, natural, and easy to follow on first hearing. Preserve this skill's stock/news pitch structure, market reasoning, source distinctions, and evidence constraints; do not replace them with the polishing skill's default point-support-takeaway structure or behavioral interview framing. Language polish must not add claims or turn a conditional forecast into a fact.

- For Sales and Trading pitches, speak directly to a client: give a clear market judgment and explain what it means for positioning, exposure, or the client's business. Keep the factual setup brief, then move naturally to the investment implication. Prefer phrasing such as "My view is...", "For your equity exposure, I'd favour...", and "The main risk to that call is..." when appropriate; vary the wording rather than repeating a template. Avoid a newspaper recap, formal essay, or classroom tour of asset classes. Client-facing delivery must not invent an existing client relationship, knowledge of the client's holdings or suitability, a house recommendation, trade sizing, or evidence of mispricing.
- Use short, speakable sentences with concrete causal explanations. Explain who benefits, who faces pressure, and why the proposed positioning follows; do not merely replace formal words with sales jargon.
- Start each numbered thesis reason with a short, plain-English takeaway, then give the evidence and explanation. Prefer a complete thought such as "First, the Fed is willing to wait" over an abstract label such as "First, policy patience." Keep the takeaway faithful to the evidence and avoid implying unanimity from a few officials' comments.
- Make the structure audible in client pitches. Use brief signposts such as "The fact is...", "My view is...", "I have two reasons", "First...", "Second...", and "For positioning..." where they help the listener follow the argument. Number the actual reasons supporting the view, keep the announced count consistent, and do not invent extra reasons to fit a template. Keep the cause of the event brief; numbered investment reasons belong with the thesis, not an expanded background section. Give each reason a concrete keyword and echo the main keywords in a short closing when useful. When the user requests a keyword summary, provide it outside the speech, in the requested language. Written headings alone do not replace spoken signposts, and signposts should not make every sentence sound mechanical.
- Avoid repeated "I would", formal essay language, generic enthusiasm, excessive jargon, and strings of three abstract nouns.
- Prefer direct, familiar wording that a listener can understand once. Replace opaque market expressions with a concrete trigger and consequence; for example, "prices could rise sharply if production is disrupted" is clearer than "prices remain vulnerable to upward spikes". Preserve the distinction between a possible spike and a sustained trend.
- Avoid compressed research phrasing and vague references. Replace "December looks more likely under my base case" with "I expect the Fed to wait until December before raising rates again." Replace "An October hold alone offers no guarantee of that outcome" with the actual outcome and reason, such as "Keeping rates unchanged in October would not necessarily lift gold prices. Future interest-rate expectations and the dollar also matter." These are wording examples, not standing market forecasts. State the causal steps in simple English; do not rely on a Chinese explanation to repair an unclear English pitch. Cut weaker asset coverage before cutting explanations needed to understand the logic.
- Explain unfamiliar sector or market terms briefly in plain language, using a short example only when helpful. Cut low-priority assets or detail before adding jargon or longer explanations.
- Make scope precise: name the institution or country providing support, distinguish loans from grants and approved funding from disbursements, and do not equate financial aid with supplier orders. Keep established facts separate from forecasts about future support.
- Use numbers selectively; each should strengthen the argument and be explainable if challenged.
- Count the words after polishing and revise until the final English pitch is no more than 250 words. Cut weaker points and repetition rather than compressing the answer into dense sentences. Do not promise an exact speaking duration.
- Keep citations outside the reusable speech. Where writing blocks are supported, place only the pitch itself in one block.
- For a final-draft-only request, return the speech with at most a brief note about remaining placeholders. Do not append a research checklist or unsolicited long/short discussion.

Before delivering, check that every material claim is supported or visibly conditional, valuation years are clear, thesis points do not duplicate valuation, and the catalyst is not fabricated. A listener should be able to state what outcome the speaker expects, why it is more likely than the main alternative, and what would invalidate it. Revise any passage that only lists important variables, explains generic asset behaviour, or proposes future research without communicating a view.
