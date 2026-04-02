---
name: blog-post
description: Biweekly blog post pipeline for unpacked by fialka
schedule: biweekly
deadline: Saturday (Kaja reviews over the weekend)
---

# Blog Post Pipeline

## Edition Numbering

Count all issues with `research` label (open + closed) to determine the latest edition. Next edition = count + 1.

## Steps (created as GitHub Issues)

### 1. Research
- **Title**: `[Edition {N}] Research: Scan travel news and topics`
- **Labels**: `worker`, `research`
- **Depends on**: none
- **Skill**: `.claude/skills/research.md`
- **Output**: `research/YYYY-MM-DD.md`

### 2. Draft
- **Title**: `[Edition {N}] Draft: Write blog post`
- **Labels**: `worker`, `draft`
- **Depends on**: Research issue for this edition (planner links by issue number)
- **Skill**: `.claude/skills/draft.md`
- **Output**: `drafts/YYYY-MM-DD-draft.md`

### 3. Review
- **Title**: `[Edition {N}] Review: Polish blog post`
- **Labels**: `worker`, `review`
- **Depends on**: Draft issue for this edition (planner links by issue number)
- **Skill**: `.claude/skills/review.md`
- **Output**: Updates draft in place

## Quality Standards

### Research
- [ ] At least 5 findings across content pillars
- [ ] Mix of myth-busting, ethical inquiry, and niche discovery topics
- [ ] Sources are credible (not influencer content or listicles)
- [ ] At least one potential Niche Bucketlist destination identified
- [ ] Topics have a genuine fialka angle (not generic travel news)

### Draft
- [ ] Title is lowercase and provocative
- [ ] Appropriate word count for type (essay ~3000, narrative ~2500-4000, bucketlist ~1800-2000)
- [ ] No em dashes
- [ ] Voice is conversational, sardonic, self-deprecating
- [ ] At least one self-implicating moment
- [ ] Personal experience woven in naturally
- [ ] Nuanced conclusion (not prescriptive)
- [ ] Would Kaja publish this under her name?

### Review
- [ ] All draft quality standards met
- [ ] Voice is consistent and sounds like fialka
- [ ] No generic travel content or influencer language
- [ ] Provocative enough to spark discussion
