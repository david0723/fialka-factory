# unpacked by fialka

Travel writing that questions everything you thought you knew about seeing the world.
Publication: https://fialka.substack.com

## Identity

**Author**: Karolina (fialka) - Czech travel writer, 31, lives in Prague with her fiance David and pet frog Ted Paul. Experience enthusiast, not a travel influencer. Backpacked 50+ countries over a decade. Former pharmaceutical chemistry student turned technical writer turned Substack writer.

**Audience**: Late 20s to mid-30s experienced travelers who've moved past the backpacker phase and are questioning their relationship with travel. They want thoughtful takes, not itineraries. Somewhat cynical about influencer culture, care about ethics but aren't performatively woke about it.

**Format**: Mix of opinion essays (~3000 words), personal narratives (~2500-4000 words), and Niche Bucketlist destination guides (~1800-2000 words).

**Publish cadence**: Every 7-14 days (biweekly average)

## Content Pillars

1. **Myth-busting** - debunking romanticized travel narratives (voluntourism, country counting, "living for free abroad")
2. **Ethical inquiry** - moral dimensions of tourism (overtourism, dual pricing, environmental impact, gentrification)
3. **Niche discovery** - researching obscure, off-the-beaten-path destinations (Niche Bucketlist series)
4. **Personal narrative** - vulnerable travel stories with emotional honesty (postcards from places)
5. **Cultural criticism** - analyzing travel industry and culture trends (TikTok itineraries, passport bros, budget travel extinction)

## How This Repo Works

This repo uses the **Depot** pattern: scheduled AI agents coordinate via GitHub Issues.

| Component | Location | Purpose |
|-----------|----------|---------|
| Agents | `.claude/agents/` | Planner, worker, and operator behavior |
| Skills | `.claude/skills/` | How to do specific tasks (research, draft, review) |
| Skill map | `.claude/SKILL_MAP.md` | Which issue labels route to which skills |
| Pipelines | `.claude/pipelines/` | Recurring task definitions and quality standards |
| Workspace | `research/`, `drafts/`, `articles/` | Where agents read and write content |
| Reference | `reference/` | Kaja's real articles for voice/style reference |
| Workflows | `.github/workflows/` | GitHub Actions schedules |
| Dashboard | `dashboard/` | GitHub Pages dashboard |

## Schedule

- **Planner**: Monday 9am UTC (creates pipeline issues, reviews quality)
- **Worker**: Every 4 hours (picks up open tasks)
- **Kaja**: Reviews output before publishing

## Operations

**Trigger manually:**
```
gh workflow run "Depot: Planner"
gh workflow run "Depot: Worker"
```

**Change config via natural language:**
Create a GitHub Issue with the `operator` label.
