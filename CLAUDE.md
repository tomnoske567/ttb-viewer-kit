# Know Your Viewer Kit — Guide for Claude

This folder is a self-contained kit that helps a creator build their **Ideal Viewer Document** — a living profile of exactly who their content is for, built from their real data plus a guided interview.

## The one job

When the user says anything like "build my viewer doc", "where do I start", "create my ICP", or "/viewer-doc" → run the skill at `.claude/skills/viewer-doc/SKILL.md` and follow it exactly.

When they say "update my viewer doc" → the skill's Update mode.

## Folder map

```
.claude/skills/viewer-doc/SKILL.md   ← The guided process. Follow it exactly.
templates/VIEWER-DOC-TEMPLATE.md     ← Document skeleton. Fill it, don't restructure it.
templates/dashboard.html             ← Dashboard shell. Fill placeholders, don't redesign.
examples/example-viewer-doc.md       ← A finished (fictional) example for reference.
my-data/                             ← Where the user drops their raw material.
MY-VIEWER.md                         ← The user's document (created by the skill).
MY-VIEWER-DASHBOARD.html             ← The user's dashboard (created by the skill).
```

## Rules that override everything

1. **Never invent data.** Every quote, number, and claim in the user's document must come from their real material or their direct interview answers. Missing evidence → mark `TO VALIDATE`.
2. **Quotes stay verbatim.** Never clean up or paraphrase the user's audience language. The raw phrasing is the value.
3. **One question at a time** during the interview. This is a conversation, not a form.
4. **The user's data stays here.** Never send the contents of `my-data/` or `MY-VIEWER.md` anywhere external.
