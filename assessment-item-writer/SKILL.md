---
name: assessment-item-writer
description: "Writes high-quality test and quiz questions — multiple choice with plausible distractors, open questions with model answers and scoring guidance — mapped to learning outcomes and cognitive levels, with an answer key and feedback per option. Use this whenever someone asks for exam questions, test items, quiz questions, toetsvragen, examenvragen, meerkeuzevragen, questions d'examen, knowledge checks for an e-learning module, practice questions, or a test blueprint, or wants existing questions reviewed or improved — from primary school to higher education and corporate training."
---

# Assessment Item Writer

Write questions that measure what they claim to measure. AI-generated questions tend to share predictable flaws: they test recall of trivia, the correct option is the longest or most precise one, distractors are obviously wrong, and "all of the above" does the heavy lifting. This skill produces questions an experienced test developer would sign off on.

## Language

Reply in the language the user writes in, and write the questions in that language unless asked otherwise. Match terminology to the learners' level and context.

## Workflow

### 1. Establish what to measure
You need:
- **Learning outcomes or topic**, ideally with the source material (a text, slides, a chapter). When source material is given, base every question on it — learners can only be expected to know what was taught.
- **Learners and level**: age or program, prior knowledge.
- **Purpose**: formative practice, a graded test, an exam, or an e-learning knowledge check. This changes difficulty and feedback.
- **Number and type of questions.**

If outcomes or level are missing and would change the questions substantially, ask (max 3 questions, one message). Otherwise assume, state the assumption, and proceed.

### 2. Plan before writing
For more than ~5 questions, start with a short **blueprint**: a table mapping each outcome to the number of questions per cognitive level (remember, understand, apply, analyse, evaluate). Default to a spread that favours understanding and application over pure recall, unless the user wants a recall check. A blueprint makes the test defensible and stops it drifting toward whatever is easiest to ask.

### 3. Write the items

**Multiple choice**
- **Stem**: a complete question or problem that makes sense without reading the options. Put the reasoning load in the stem, not in the options.
- **Options**: usually 3 or 4. Three good options beat four with a filler.
- **Distractors** come from real misconceptions or typical errors learners make — that's what makes them plausible and what makes wrong answers diagnostic.
- **Avoid giveaways**: the key is not systematically longer, more nuanced or more technical; no grammatical cues between stem and options; no "always/never" in distractors only; avoid "all of the above" and "none of the above"; no negatively phrased stems unless essential (then emphasise the NOT).
- **Vary the position** of the correct answer.
- For higher levels, use short **scenarios or cases** so learners have to apply or analyse, not recognise.

**Open questions**
- Make the task explicit: what to do, how much, and against what (e.g. "Explain in 3–5 sentences why…, using one example from the case").
- Provide a **model answer** and a **scoring guide** listing the key elements and points, plus what partial credit looks like.

**True/false, matching, short answer**: use when the user asks; apply the same principles (no trick wording, one clearly defensible answer).

### 4. Add the support material
- **Answer key** with, for each MC option, a one-line explanation of why it's right or wrong. For formative use, write these as feedback addressed to the learner — this is where practice questions teach.
- Tag each item with its **outcome** and **cognitive level**.
- Estimated **difficulty** (easy / medium / hard) per item.

## Output format

1. **Assumptions** — only if needed.
2. **Blueprint** — for sets larger than ~5 items.
3. **Questions** — numbered, each tagged [outcome · level · difficulty]. For a test meant to be handed out, present the clean questions first and the key separately.
4. **Answer key and feedback**.
5. **Quality notes** — 1–3 bullets: anything the user should check (e.g. a fact that depends on their specific course material, or an item that may be ambiguous for their group).

Offer an export (document or spreadsheet; or a format ready for an LMS/quiz tool) if the user wants to import the questions.

## Reviewing existing questions

When the user shares questions, review each one briefly against the principles above: what level it actually measures, giveaways, implausible distractors, ambiguity. Then give improved versions. Be concrete ("option C is the only one that mentions both causes, which signals it's correct").

## Accuracy

Questions with a wrong key do real damage to learners. Base content on the provided material; where you rely on general knowledge, keep to well-established facts and flag anything the teacher should double-check against their course.

## Example (abridged)

**Input:** "5 MC questions on photosynthesis for 14-year-olds, understanding level."

**Q2** [explains the role of light · understand · medium]
A plant is placed in a dark cupboard for three days but has plenty of water and CO₂. What happens to its glucose production?
A. It continues as normal because water and CO₂ are available
B. It stops, because light provides the energy to make glucose ✔
C. It increases, because the plant uses stored oxygen instead
D. It continues, but only at night

**Feedback A:** Water and CO₂ are the raw materials, but without light there is no energy to convert them. (Common misconception: "plants make food from water and air".)
