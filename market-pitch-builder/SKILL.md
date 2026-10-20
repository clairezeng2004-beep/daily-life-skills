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
- Keep each final English pitch at or below 250 words, including any headings within the pitch; follow a shorter requested limit when supplied. Keep research notes and citations outside the spoken pitch. Put the Chinese keyword summary and causal chains before the English speech in the same writing block; they do not count toward the English word limit. Expand supporting material only when requested.
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

Use four visible section labels in this order, with a colon after each: `Fact:`, `Why it happened:`, `Market impact:`, `My view:`. Keep labels accurate to the section's purpose and inside the English pitch's word count. Follow a different structure when explicitly requested.

1. **Fact:** State what happened in exactly one sentence, including the relevant timing and parties. Keep causes, forecasts and personal judgments out of this sentence.
2. **Why it happened:** Explain two or three distinct, evidence-grounded causes of the event or observed market reaction. Use short spoken signposts such as "First" and "Second". Do not repeat one cause in different words or substitute reasons for the investment recommendation. If fewer causes are supported, say so rather than inventing an extra cause. Identify interpretations outside the speech when they are not established by the source.
3. **Market impact:** Choose only assets, products, sectors or companies with a meaningful connection to the event; do not require gold, commodities or multiple asset classes. A focused equity-only discussion is acceptable. Start each material impact with a clear direction, such as "This is negative for manufacturers that depend on imported yttrium," then explain the full chain from the event to costs, production, deliveries, earnings or discount rates and finally to prices. Do not imply that a negative earnings effect guarantees a share-price decline regardless of existing expectations. For cross-border effects, name the dependency: for example, a shortage delays Japanese components, so overseas customers cannot complete their own products on schedule. Merely listing industries or countries is not a causal explanation. Separate observed moves from expected effects. Where direction is unsupported, omit the asset or explicitly state the narrow uncertainty instead of forcing a call. Keep personal preferences such as "I favour" and trade recommendations in My view, not in this section. Use a short spoken transition only when it helps.
4. **My view:** Finish with an explicit judgment: is the event, trend or market reaction likely to continue, and is the pricing response reasonable? Explain why, over a source-supported horizon where available, and state what would invalidate the judgment. Distinguish a justified repricing from evidence that a security is cheap or expensive; do not invent valuation or consensus evidence. For policy-driven shortages, assess whether restrictions are likely to ease and why, using evidence about negotiations, implementation of prior pledges and incentives. Distinguish a partial concession from broad normalisation; do not claim a verified timetable when none exists. Monitoring points should test this judgment, not replace it.

Keep the causal explanation, cross-asset implications and personal assessment in their respective sections. Do not revert to the previous three-section Fact / My view / Impact structure.

### Copyable bilingual delivery

For each finished news pitch, put a concise Chinese keyword summary and causal chains at the top of the same writing block as the English speech. Organise the Chinese notes around the same four stages: fact, causes, cross-asset impact and personal judgment. Use arrows where they clarify causality. Put the topic title inside the block, followed directly by the Chinese notes without a redundant "中文关键词和逻辑链" heading. Put source links and brief evidence qualifications at the bottom of the same block, clearly separate from the spoken English; they do not count toward its word limit. The English must remain understandable without the Chinese notes. If writing blocks are unavailable, keep the Chinese notes and English pitch together in one clearly delimited copyable section. For several pitches, use one block per pitch within the platform's block limit.

Separate observed price reactions from expected future reactions. Distinguish announcement date from effective date. Describe a consensus disagreement only if expectations are evidenced. Do not force a trade recommendation into a request for news interpretation alone.

## Spoken style and delivery

Before delivering a final pitch, read and apply [video-interview-answer-polisher](../video-interview-answer-polisher/SKILL.md) from this repository. Use its spoken-language editing and final quality check to make the English clear, natural, and easy to follow on first hearing. Preserve this skill's stock/news pitch structure, market reasoning, source distinctions, and evidence constraints; do not replace them with the polishing skill's default point-support-takeaway structure or behavioral interview framing. Language polish must not add claims or turn a conditional forecast into a fact.

### Spoken sentence standard

The user prefers natural interview speech over written research prose. Treat this as a delivery requirement, including when the investment logic is technically complex.

- Avoid repeated participial add-ons such as ", raising concerns...", ", making investors..." and ", leaving bondholders...". Use a complete sentence with a named subject and verb, or a short because/so clause that makes the causal relationship explicit. For example: "Borrowing costs rose. Investors became more concerned about profits." Preserve whether causality is established or inferred.
- Avoid chains of -ing phrases and gerund-led abstract subjects. Do not ban ordinary market terms such as earnings, financing or pricing, or natural progressive verbs merely because they end in -ing.
- Aim for most sentences to be about 10–20 words. Review sentences over 25 words, nested relative clauses, and sentences with several qualifications. Split at a natural idea boundary without losing material conditions or turning the speech into disconnected fragments.
- Prefer familiar verbs and concrete explanations: "The company needs to borrow more" instead of "The business faces greater funding requirements"; "Other lenders get paid first" instead of "There are substantial claims ahead of the unsecured debt". Keep a technical term when it helps, and explain it briefly.
- Read each English pitch aloud mentally before delivery. Rewrite sentences that sound like a research report, or that require the listener to remember several clauses before understanding the point. Preserve the four news sections, first-person judgment and source fidelity. The Chinese notes must not compensate for unclear English.

### Source language and client comprehension

- Prefer financial terms and natural collocations already present in the reports read for this pitch, or established financial-market expressions. Do not invent terminology, unusual word pairings, compressed labels or slogans to sound sophisticated. When neither source wording nor a familiar market expression is clear, use ordinary English to explain the mechanism.
- During reading, note a few useful source expressions alongside their meaning and source location. Reuse short conventional expressions accurately, not distinctive sentences or extended passages. Source wording is a vocabulary guide, not a requirement to copy written research language. Preserve attribution and quotation limits; never imply that an original synthesis was the report's conclusion.
- Retain useful standard terms such as forward P/E, capital expenditure and free cash flow when relevant. Explain an unfamiliar term briefly on first use. A client should understand who spends the money, who receives it and what changes for profits or the stock price without knowing the terminology beforehand.
- Minimise lists of parallel words and phrases, especially abstract nouns and repeated three-part lists. Choose the most important driver and explain its consequence. Give a second driver its own sentence only when it adds a distinct argument. Do not replace a three-item list with several equally unexplained fragments, and do not remove material qualifications just to shorten a list.
- Prefer a concrete explanation over a research-style summary. For example, replace "cash generation and delivery should matter more for returns" with "I'd favour companies able to fund their own investment. They depend less on new borrowing." Replace "execution and funding risks" with "A delayed project starts earning revenue later. The developer may need to borrow more in the meantime." These are wording examples, not standing investment recommendations or additional source evidence.
- Before delivery, check each technical expression: is it used in the source or standard in markets, is its meaning accurate here, and can the intended client understand the sentence on first hearing? Rewrite unfamiliar combinations in ordinary English. Check lists separately and remove stacked drivers without an explained causal link. When asked about wording provenance, distinguish source expressions, standard market language and the assistant's own paraphrases candidly.

### Delivery checks

- For Sales and Trading pitches, speak directly to a client: give a clear market judgment and explain what it means for positioning, exposure, or the client's business. Keep the factual setup brief, then move naturally to the investment implication. Prefer phrasing such as "My view is...", "For your equity exposure, I'd favour...", and "The main risk to that call is..." when appropriate; vary the wording rather than repeating a template. Avoid a newspaper recap, formal essay, or classroom tour of asset classes. Client-facing delivery must not invent an existing client relationship, knowledge of the client's holdings or suitability, a house recommendation, trade sizing, or evidence of mispricing.
- Use short, speakable sentences with concrete causal explanations. Explain who benefits, who faces pressure, and why the proposed positioning follows; do not merely replace formal words with sales jargon.
- Start each numbered thesis reason with a short, plain-English takeaway, then give the evidence and explanation. Prefer a complete thought such as "First, the Fed is willing to wait" over an abstract label such as "First, policy patience." Keep the takeaway faithful to the evidence and avoid implying unanimity from a few officials' comments.
- Make the structure audible in client pitches. Use brief signposts such as "The fact is...", "My view is...", "I have two reasons", "First...", "Second...", and "For positioning..." where they help the listener follow the argument. Number the actual reasons supporting the view, keep the announced count consistent, and do not invent extra reasons to fit a template. For news pitches, number the distinct causes in Why it happened, explain asset transmission in Market impact, and reserve the continuation and reasonableness judgment for My view. Keep all four sections concise. Give each reason a concrete keyword and echo the main keywords in a short closing when useful. Keep Chinese keywords and causal chains outside the English speech but inside the same writing block, before the speech. Written headings alone do not replace spoken signposts, and signposts should not make every sentence sound mechanical.
- Avoid repeated "I would", formal essay language, generic enthusiasm, excessive jargon, and strings of three abstract nouns.
- Prefer direct, familiar wording that a listener can understand once. Replace opaque market expressions with a concrete trigger and consequence; for example, "prices could rise sharply if production is disrupted" is clearer than "prices remain vulnerable to upward spikes". Preserve the distinction between a possible spike and a sustained trend.
- Avoid compressed research phrasing and vague references. Replace "December looks more likely under my base case" with "I expect the Fed to wait until December before raising rates again." Replace "An October hold alone offers no guarantee of that outcome" with the actual outcome and reason, such as "Keeping rates unchanged in October would not necessarily lift gold prices. Future interest-rate expectations and the dollar also matter." These are wording examples, not standing market forecasts. State the causal steps in simple English; do not rely on a Chinese explanation to repair an unclear English pitch. Cut weaker asset coverage before cutting explanations needed to understand the logic.
- Explain unfamiliar sector or market terms briefly in plain language, using a short example only when helpful. Cut low-priority assets or detail before adding jargon or longer explanations.
- Make scope precise: name the institution or country providing support, distinguish loans from grants and approved funding from disbursements, and do not equate financial aid with supplier orders. Keep established facts separate from forecasts about future support.
- Use numbers selectively; each should strengthen the argument and be explainable if challenged.
- Count the words after polishing and revise until the final English pitch is no more than 250 words. Cut weaker points and repetition rather than compressing the answer into dense sentences. Do not promise an exact speaking duration.
- Keep citations outside the spoken English, at the bottom of its writing block. Include the topic title, Chinese keywords and causal chains, English pitch, and source links together so the user can copy the complete material.
- For a final-draft-only request, return the speech with at most a brief note about remaining placeholders. Do not append a research checklist or unsolicited long/short discussion.

Before delivering, check that every material claim is supported or visibly conditional, valuation years are clear, thesis points do not duplicate valuation, and the catalyst is not fabricated. A listener should be able to state what outcome the speaker expects, why it is more likely than the main alternative, and what would invalidate it. Revise any passage that only lists important variables, explains generic asset behaviour, or proposes future research without communicating a view.
