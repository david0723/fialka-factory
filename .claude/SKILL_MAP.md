# Skill Map

Routes issue labels to skill files.

| Label | Skill File | Description |
|-------|-----------|-------------|
| `research` | `.claude/skills/research.md` | Gather travel news, ethical tourism stories, niche destinations |
| `draft` | `.claude/skills/draft.md` | Write blog post draft in fialka's voice |
| `review` | `.claude/skills/review.md` | Quality check and polish |

## Notes

- Every `worker`-labeled issue must also have exactly one skill label.
- If an issue has an unknown label, the worker comments asking for clarification and skips it.
- The `writing-style.md` skill is a reference document, not directly routable. It's read by draft and review skills.
