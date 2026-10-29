# LR17 — Review of the student's repeat manual analysis

Date: 2026-10-29. The student reported 19 minutes manual analysis, 16 minutes AI interaction, and 4 minutes review. Original source: `manual-analysis(1).txt` uploaded in the conversation. AI reference: P-02 in `lr17_ai_assistant/README.md` at `stkossman/it-project-management`.

**Integrity:** This human-written exercise took place *after* the student had previously been exposed to AI analysis of the same notes. It is not a pre-AI independent baseline for LR17 block C. Preserve the original manual file unedited. This file documents a retrospective comparison only.

## Pairwise comparison (original 12 manual lines)

| Manual ID | Source tag | Manual type/meaning (abbreviated) | P-02 overlap | Assessment |
|---|---|---|---|---|
| M01 | N-01,N-14 | decision: teacher is main user, acceptance during live class | N-14 decision | Overlap through N-14 only. N-01 identifies the customer but is context, not a separate adopted decision. |
| M02 | N-03 | decision: release by November 28 | N-03 decision | Match; year is not specified in the educational notes. |
| M03 | N-06 | decision: no named students in public statistics | N-06 decision | Match. |
| M04 | N-02 | task: make cards larger/readable on projector | N-02 task | Match, with a suggested UI solution rather than a measured size requirement. |
| M05 | N-04 | task: account for approximately 20 sessions per semester | None of same tag and type | Human-only candidate; N-04 contains forecast/context, not an explicitly agreed task. Verify whether to treat as proposed capacity-planning action rather than accepted requirement. |
| M06 | N-04,N-11,N-13 | task: guarantee minimum 30 simultaneous users and load-test | None of same type | Human-only candidate, but incorrectly promotes a disputed 25/30 count to an agreed minimum. Rewrite as open question about the target and proposed performance test **only if clearly marked as a proposal**, not as an approved requirement. |
| M07 | N-09 | task: check WebSockets across buildings and fallback | N-09 task | Match; fallback is a proposed response. The notes say only one classroom was tested. |
| M08 | N-10 | task: export variance statistics for validator | N-10 task | Match; precise schema is unknown and not yet approved for REL-1. |
| M09 | N-12 | task: persist voting results | N-12 task | Match. |
| M10 | N-05 | open_question: late join behavior and owner | N-05 open_question | Match. P-02 also includes a separate N-05 task. |
| M11 | N-07 | open_question: retain or purge semester sessions | N-07 open_question | Match. |
| M12 | N-08 | open_question: moderator if teacher absent | N-08 open_question | Match. |

**Descriptive totals:** 12 manual formulations; 16 P-02 formulations; 10 tag-and-type matches; 2 human-only candidates requiring source qualification; 6 AI-only distinct tag-and-type items. These are retrospective comparison counts, **not** official `origin=mine/ai/both` provenance for the pre-AI exercise.

## Six P-02 items without a matching manual tag-and-type item

1. N-04 / open_question: decide participant capacity limit (25 vs. 30).
2. N-05 / task: specify late-join behavior (manual captured the question, not an explicit task line).
3. N-09 / open_question: determine which buildings remain untested for WebSocket restrictions.
4. N-10 / open_question: obtain the exact validator export schema.
5. N-11 / open_question: confirm whether 30 participants is an acceptance scenario.
6. N-13 / open_question: determine why the previous two services reportedly failed at 20 participants.

## Timing evidence (self-reported)

- Manual: 19 minutes.
- AI interaction: 16 minutes.
- Human review: 4 minutes.
- Arithmetic: `19 - 16 - 4 = -1` minute (AI plus review took 20 minutes, one more than manual).
- **Comparability limitation:** The manual work was after earlier exposure to P-02. Confirm whether the 16-minute AI and 4-minute review were measured for the same task and by what method before recording this as a `measured` `time_saved.csv` row. Do not attribute these times to the original historical P-01/P-02 unless genuine evidence exists.

If the user confirms stopwatch-style measurement and comparable task, candidate CSV row:

```csv
case_id,task,basis,minutes_manual,minutes_ai,minutes_review,minutes_saved,how_measured
TS-01,"Повторний розбір нотаток Planning Poker після ознайомлення з AI",measured,19,16,4,-1,"Повідомлені студентом заміри 2026-10-29: ручний аналіз 19 хв; AI 16 хв; перевірка 4 хв. Повторна вправа після попереднього AI-ознайомлення; не pre-AI baseline."
```

The course requires three complete cases and at least one measured case; only one candidate case is currently available. Never fabricate two others.

## Next steps

- Preserve the untouched manual file as a separate, transparently labeled student-authored record; keep it outside the university portfolio until the student chooses to include it and its date/provenance are made explicit.
- Present the retrospective comparison in LR17 README without falsely declaring the independent pre-AI block completed.
- Ask the instructor whether a fresh exercise on a different, approved Planning Poker dataset may substitute for the original pre-AI baseline.
- Keep the P-02 source output unchanged and preserve `tasks.csv` origin history until provenance can be represented truthfully.
