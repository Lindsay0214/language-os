# Language OS Daily Workflow

Use this template when the user says `Start Day N`. Include a time budget beside every section and keep the total mission manageable.

## 1. Generate Today's Mission

Create a manageable mission with one task in each required area:

Default time budgets:

- English Listening — 10 minutes
- IELTS Speaking — 25 minutes
- English Writing — 20 minutes
- Grammar and sentence repair — 15 minutes
- German Lesson — 10 minutes
- German Guided Practice — 10 minutes
- German Mini Output — 5 minutes

For the two weeks after Day 2, use this adaptive allocation unless the user requests a different focus. Keep speaking sentences focused on one main idea, add five high-frequency IELTS items, and include a short German A1 lesson every day.

### English

#### Listening

Use a short, level-appropriate listening activity from a real, accessible source. Include:

- source title;
- publisher or creator;
- direct playable URL;
- expected listening length;
- whether the user should listen once or twice.

Ask for a summary, key details, or a transcript-based recall response. Use a generated passage only when a real source is unavailable or the user requests one.

#### IELTS Speaking

Choose an IELTS-style Part 1, Part 2, or Part 3 prompt. Ask the user to answer in English and state the target response length.

#### Writing

Choose a focused English writing task. State the purpose, audience, length, and any IELTS task requirements.

### German

German is teaching-first for this beginner. Teach one small A1 concept before asking for output.

#### Lesson

Teach one small concept such as greetings, `sein`, `haben`, numbers, or simple word order. Explain it in plain English, show 3–5 model sentences with translations, and highlight only the essential pattern.

#### Guided Practice

Give 3–5 supported exercises such as choosing a word, completing a sentence, or translating a very short phrase. Show the allowed vocabulary and do not test an unexplained concept.

#### Mini Output

Ask for only 2–3 original German sentences using the lesson pattern. State that mistakes are expected and that the learner may use the model vocabulary.

## 2. Wait for Answers

Present the mission, then stop and wait. The user may answer with headings such as:

```markdown
## English Listening

...

## IELTS Speaking

...

## English Writing

...

## German Vocabulary

...

## German Speaking

...

## German Writing

...
```

Do not review, score, or update files before the user submits answers. If the user submits only some sections, review only those sections and mark the rest incomplete.

## 3. Review Every Answered Section

For each answered section, provide:

1. a score or concise rating;
2. what worked;
3. the original answer or a clearly identified excerpt;
4. corrected language;
5. the most important explanation;
6. one repetition task.

For English speaking and writing, also provide sentence-level corrections and a polished natural version. Keep the daily review focused on the most important patterns; reserve exhaustive line-by-line teaching for a specialist follow-up when requested.

For IELTS speaking and writing, comment on task response, coherence, vocabulary, grammar, and fluency or accuracy as applicable. For German, explain case, gender, word order, or conjugation errors when relevant. For listening, separate comprehension evidence from language-production errors.

For German beginner work, review the lesson understanding and supported practice before judging original output. Do not penalize the learner for not producing unsupported language, and do not add copied model sentences to the mistake database.

## 4. Capture Learning Data

Extract only supported items:

- Anki candidates: phrase, meaning, example, and a short recall prompt;
- mistakes: the user's form, corrected form, explanation, and a future practice cue;
- vocabulary: the word or phrase, meaning, context, and example.

Prefer recurring, high-value items over a long list.

## 5. Update the Repository

After review:

1. update today's `journal/YYYY/MM/YYYY-MM-DD.md` using `templates/daily.md`;
2. update `mistakes/english.md` and/or `mistakes/german.md`;
3. update `vocabulary/english.md` and/or `vocabulary/german.md`;
4. update the README streak only when the session qualifies under `rules.md`;
5. show a concise summary of every changed file.

Never invent answers, scores, vocabulary, or study duration. Keep unanswered work visibly incomplete.

## 6. Commit

If the session produced repository changes, create one commit using:

```text
Study YYYY-MM-DD: English and German practice
```

Do not include unrelated files in the commit. Report the commit hash and the final streak after committing.
