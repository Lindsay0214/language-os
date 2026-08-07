# Repository-Driven Daily Workflow Design

## Goal

Make the Language OS repository the source of truth for recurring daily language-coaching sessions. A user should be able to start a session with a short command such as `Start Day 2`, answer tasks inside the workspace, and receive a complete review plus repository updates without re-pasting the workflow.

## Components

### `AGENTS.md`

The root-level operating guide will define the stable contract for Codex:

- learning goals: IELTS English and practical German;
- required daily workflow and answer format;
- review responsibilities and reference documents;
- files that may be updated after a completed session;
- content and files that must not be changed without explicit reason;
- commit-message convention.

It will reference the existing `rules.md`, `templates/daily.md`, and language-specific mistake and vocabulary files. It will also identify `review-standard.md` as the preferred review source if that file is added later.

### `templates/day-prompt.md`

The daily template will define the execution sequence:

1. Generate English listening, IELTS speaking, and English writing tasks.
2. Generate German vocabulary, German speaking, and German writing tasks.
3. Wait for the user's answers before reviewing.
4. Review every completed section, score performance, correct language, and explain the highest-value issues.
5. Extract useful vocabulary and Anki candidates.
6. Update the dated journal, mistakes database, vocabulary, and README streak.
7. Show the changed files and create one dated Git commit.

The template will require the coach to preserve unanswered sections, distinguish user answers from corrections, and avoid inventing study evidence.

## Data Flow

`Start Day N` loads `AGENTS.md`, which points to `templates/day-prompt.md` and the supporting rules. Codex generates a mission and waits. After the user submits answers, Codex reviews the answers, records durable learning data in the existing Markdown stores, updates the journal and streak, then commits the session changes.

## Safety and Scope

- Existing Day 1 records remain unchanged.
- The daily journal remains date-based and uses the existing template conventions.
- Mistakes and vocabulary are added only when supported by the user's work or explicit review.
- No external app, hidden database, or new file format is introduced.
- A missing `review-standard.md` is handled by the documented fallback to `rules.md` plus the review checklist in `AGENTS.md`; Codex should not claim to have followed a file that does not exist.

## Verification

Self-review checks will confirm that the two new files name the same workflow, point to real existing paths, preserve the two-phase wait-and-review behavior, and provide an explicit commit rule.
