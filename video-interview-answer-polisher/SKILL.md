---
name: video-interview-answer-polisher
description: Turn Chinese or English interview notes into concise, natural spoken English answers for video interviews, with time-aware word counts and non-AI-sounding phrasing.
---

# Video Interview Answer Polisher

Use this skill when the user is preparing spoken English answers for video interviews, HireVue-style applications, recorded interview questions, or short application videos. The user may provide Chinese notes, English drafts, mixed-language thinking, or a rough structure.

This skill is more speech-focused than `application-answer-polisher`. Use it when the user gives or implies an answer duration, asks for more oral/conversational wording, or wants the response to sound natural when spoken aloud.

## Timing

Default to 80-120 words per minute unless the user gives a different pacing preference.

- For 30 seconds, write around 45-65 words.
- For 1 minute, write around 80-120 words.
- For 1.5 minutes, write around 130-170 words.
- For 2 minutes, write around 170-230 words.

Stay slightly under the upper limit when the answer includes names, technical terms, numbers, or phrases the user may want to say carefully.

## Core Delivery Requirements

Conversational delivery and the absence of formulaic AI phrasing are acceptance criteria, not optional polish. Write for a listener who hears the answer once.

- Use everyday verbs, natural contractions, and sentences that fit a comfortable breath. Preserve useful technical terms and explain their practical meaning simply.
- Prefer "What draws me to MS is..." to "These capabilities underpin my interest...". Describe what a client or candidate can actually do.
- Vary sentence length and openings. Avoid corporate abstractions, polished symmetry, repeated three-part lists, and slogan-like endings.
- Keep evidence precise without reciting full report titles or stacking rankings. Prefer one memorable example with a short attribution.
- Never invent experiences or exaggerate evidence to create an engaging hook.

## Spoken Sentence Standard

- Aim for most sentences to be 8-16 words. Review every sentence over 20 words and usually split or simplify it. These are editing guides, not a reason to make speech choppy or delete useful detail.
- Give each sentence one main idea. Put an explanation or consequence in the next sentence when it adds another clause.
- Prefer direct personal language such as "I like", "I enjoy", and "I'd like to" when it fits the user's voice. Do not replace natural wording with a formal motivational introduction just to sound polished.
- Use concrete verbs instead of noun-heavy phrases: "I like following markets" is easier to say than "What draws me is the combination of market engagement and relationship building".
- Shortening alone is insufficient. Check that the words sound like something the candidate would say in conversation with an interviewer. Avoid turning every sentence into a formal declaration or a slogan.
- Preserve natural wording while keeping a short opening that names the main reason or keywords. End with one short sentence that brings those keywords back to the motivation or lesson. Short sentences should not remove the answer's overall structure.
- Keep related short sentences together in natural paragraphs. Do not put each sentence on a separate line or add pauses and performance directions unless requested.

Example of the intended revision:
- Too written: "That constant feedback keeps me engaged, because I have to question my assumptions and decide when to hold my view or adjust it."
- Spoken: "I like getting that constant feedback. It makes me question my assumptions. Sometimes I stick with my view; sometimes I change it."

## Output Style

Write polished spoken English that sounds like a thoughtful candidate speaking to a camera.

- Preserve the user's facts, story, and intended strengths.
- When the user provides a draft, prefer light editing over rewriting from scratch unless they ask for a full rewrite.
- Keep the user's original order and wording where it already works.
- Preserve enough specific detail to make the answer credible. Do not flatten a technical or market answer into generic interview language.
- Make the answer clear enough to say in one take.
- Prefer short sentences and light transitions.
- Avoid long openings. For most answers, make the first sentence direct and under 20 words.
- Minimize subordinate clauses. Split sentences when a listener may lose the point.
- Avoid too many parallel nouns or repeated list structures. Several paired or three-part lists in a row can sound AI-written.
- Accept and preserve conditional phrasing such as "I would", "my first step would be", and "I would focus on" for hypothetical, market-view, or plan-of-action prompts. It sounds natural and appropriately cautious in those answers.
- Use natural spoken phrasing without fillers such as "you know", "like", or "basically".
- In English answers, use straight ASCII quotation marks (`"` and `'`) and apostrophes, including contractions such as `I'll` and `I'd`. Do not use curly quotation marks or curly apostrophes (`“ ” ‘ ’`) or Chinese quotation marks (`「 」 『 』`).
- Avoid corporate slogans, exaggerated enthusiasm, and generic claims.
- Avoid writing that sounds like a memorized essay.
- Do not over-connect every answer to the target role. Add a role connection only when it feels natural or the prompt asks for it.
- Make behavioral answers easy to follow by ear. The interviewer should remember one clear scene, problem, action, and result.

## Handling Chinese or Mixed Notes

When the user provides Chinese ideas, translate meaning rather than sentence structure.

- Convert broad Chinese claims into specific English actions where possible.
- Keep the user's original emphasis, especially the strengths they explicitly want to show.
- If a point is useful but too abstract, express it through what the user did, noticed, changed, or learned.
- If the draft has too many ideas for the time limit, keep the strongest story thread and remove weaker supporting details.
- If the user says the previous version changed too much, revise locally: keep their structure, most examples, and core sentences, then improve grammar, rhythm, and naturalness.
- If the user provides professional terms, keep the terms that carry real meaning. Explain or simplify around them instead of deleting them all.

## Competency Signposting

For behavioral interview answers, actively but naturally show desirable qualities through verbs, choices, and concrete situations. Useful qualities include:

- leadership
- ownership
- attention to detail
- collaboration and teamwork
- communication
- trust-building
- client focus
- adaptability
- commercial awareness
- problem-solving

Do not simply stack these words in a list. Anchor them in the user's actions.

Good patterns:
- "I took the lead in building a portrait photography studio at university."
- "I led the weekly planning and made sure each client knew what to expect before the shoot."
- "That taught me how to build trust quickly, especially when someone felt nervous in front of the camera."
- "It also made me think more commercially, because I had to balance pricing, equipment costs and return on investment."

Avoid:
- "This experience improved my leadership, teamwork, communication, adaptability and commercial awareness."
- "I am a detail-oriented, collaborative and highly motivated person."

## Structure

Default to point–support–takeaway (总分总), unless the user requests another format or the question clearly calls for something else. Keep the opening and closing brief and spoken; sentence simplicity and overall structure must work together:

1. **Point:** Answer immediately with one short sentence naming the main theme or one or two memorable keywords. For two reasons, give a brief spoken roadmap so the listener knows what to listen for.
2. **Support:** Develop one or two reasons with concrete evidence or a brief story. Explain why each example matters.
3. **Takeaway:** Close with one short sentence that echoes the opening keywords and connects them to the motivation, implication, or lesson. Keep the connection concrete; avoid a slogan or a word-for-word recap.

For behavioral questions, place situation, action and result inside the supporting story. Open with the behavior being asked about and close with what the experience showed or taught. Do not display STAR or structure labels in the finished script. Do not force a role connection into unrelated personal questions.

## Listener Signposts and Keywords

Help the listener follow the answer and remember its key ideas:

- Choose one or two concrete keywords, such as "stock borrowing", "execution", or "client trust". Introduce them early, develop each with evidence, and echo the main idea naturally in the takeaway.
- Use short audible cues at meaningful transitions: "The first is...", "The other is...", "One example is...", "What matters here is...", or "That's why...". Use only those needed; avoid a fixed sequence in every answer.
- Keywords should organize real content. Do not stack competency buzzwords, manufacture dramatic hooks, or make unsupported claims to attract attention.
- Keep signposts within natural sentences. Bold formatting and numbered headings cannot substitute for cues a listener can hear.

For "Tell us something about yourself that is not on your resume", focus on a memorable personal story first. A concise leadership signal in the opening is useful, such as "I took the lead in..." or "I helped build...". Mention transferable strengths, but avoid ending with an overly formal job pitch unless the user asks for that connection.

## Editing Rules

- Quietly fix grammar, collocations, and tense.
- Replace stiff phrases with native spoken English.
- Preserve vivid user details when they help the story stick, such as a client's nervousness, direct feedback, a concrete tool, monthly revenue, or ROI thinking.
- Preserve useful technical detail when it supports the answer, such as collateral quality, liquidity mismatch, refinancing risk, senior secured loans, covenants, or recovery value. Make the terms speakable rather than removing them.
- Cut repeated setup and low-value background.
- Remove dense lists of abstract nouns.
- Reduce parallel wording. Rewrite strings like "collateral opacity, liquidity mismatches, and over-concentration" into one main point plus a sentence of explanation, unless the prompt explicitly asks for a list.
- Use capability words sparingly. Prefer "took the lead", "managed client communication", "built trust", "paid attention to small details", and "thought about return on investment" over a plain list of strengths.
- Do not over-edit away repeated "would" in hypothetical answers. Vary sentence rhythm where useful, but keep "would" when it makes the answer sound measured rather than overconfident.
- Avoid template contrasts such as "not only..., but also...", "rather than...", "more than just...", "both...and...", and "instead of simply..." unless the user explicitly asks to preserve them.
- Before finalizing, read the answer mentally as speech. If it would be hard to say naturally, shorten or split the sentence.

## Response Format

Usually provide:

- A polished answer in English.
- A brief note on word count or speaking time.
- A short explanation in Chinese of what was strengthened, when useful.

When the user only asks for the answer, keep extra commentary minimal.

## Final Spoken Quality Check

Before returning the answer:

- Read it mentally aloud. Rewrite sentences that sound like an annual report, written essay, or memorized template. Review sentences over 20 words; check that most sentences are around 8-16 words and carry one main idea.
- Compare with the original draft. Remove any newly added formal framing that makes a simple personal point harder to say. Short sentences must still sound natural together.
- Check for a brief keyword-led opening, concrete support, and a short closing that returns to those keywords. A distracted listener should be able to recover the main point from the opening or closing. Do not drop this structure merely to shorten sentences.
- Check that a listener can identify the main keywords after hearing the answer once without seeing formatting.
- Remove abstract noun clusters, mechanical transitions, generic praise, and unnecessary technical detail while preserving the strongest example.
- Check the actual word count and speaking time. Cut weaker points instead of squeezing them into dense sentences.
