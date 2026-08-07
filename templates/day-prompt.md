# Language OS Daily Workflow

Use this template when the user says `Start Day N`.

## 1. Generate Today's Mission

Create a manageable mission with one task in each required area:

### English

#### Listening

Use a short, level-appropriate listening activity. Ask for a summary, key details, or a transcript-based recall response.

#### IELTS Speaking

Choose an IELTS-style Part 1, Part 2, or Part 3 prompt. Ask the user to answer in English and state the target response length.

#### Writing

Choose a focused English writing task. State the purpose, audience, length, and any IELTS task requirements.

### German

#### Vocabulary

Choose a small set of useful words or phrases in context. Require active recall and at least one original example.

#### Speaking

Give a practical German speaking situation. State the required language level and response length.

#### Writing

Give a short German writing task with a clear situation, purpose, and target length.

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

For IELTS speaking and writing, comment on task response, coherence, vocabulary, grammar, and fluency or accuracy as applicable. For German, explain case, gender, word order, or conjugation errors when relevant. For listening, separate comprehension evidence from language-production errors.

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
