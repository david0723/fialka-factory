# unpacked by fialka - AI Writing Assistant

Hey Kaja! This is your AI writing assistant. It helps you create blog content by doing the boring parts (research, first drafts, SEO) so you can focus on what you're good at: writing with your voice and connecting with your audience.

## What does this thing do?

You have a team of AI helpers that work in the background:

- **The Planner** wakes up every Monday and creates a to-do list for the week (as GitHub Issues)
- **The Worker** checks every few hours if there's anything to do, and does it (research, drafts, etc.)
- **The Operator** listens to YOU - when you want to change something, you just tell it in plain English

You don't need to understand how any of this works under the hood. You just need to know three things:

## The 3 things you need to know

### 1. Where to find the stuff it creates

| What | Where | What to do with it |
|------|-------|--------------------|
| Research notes | `research/` folder | Read before writing. Cherry-pick the good stuff. |
| Draft articles | `drafts/` folder | Edit heavily. Add your personal stories. Make it yours. |
| Your dashboard | [dashboard link](https://david0723.github.io/fialka-factory/) | Check what's been happening |

### 2. How to tell it what you want

Go to the [Issues tab](https://github.com/david0723/fialka-factory/issues) and create a new issue. Add the purple **operator** label. Then just write what you want in plain English.

**Examples of things you can say:**

- "I want to write about overtourism in Prague this week"
- "The research has been too generic, focus more on ethical travel controversies"
- "Add a new search topic: slow travel movement"
- "Make the drafts shorter, around 2000 words instead of 3000"
- "What topics are trending in travel right now?"
- "Run the worker now, I need research today"

The AI will read your request, make the changes (or ask you questions if it's not sure what you mean), and close the issue when done.

### 3. How to review and publish

The AI writes first drafts. They will sound like you (it studied your writing style), but they're NOT ready to publish as-is. Think of them as a very thorough starting point.

**Your review process:**
1. Check your [dashboard](https://david0723.github.io/fialka-factory/) or the `drafts/` folder
2. Open the draft
3. Add your personal stories and anecdotes (the AI can't make these up)
4. Fix anything that doesn't sound like you
5. Add your photos
6. Publish on Substack as usual

**The AI will never publish anything on its own.** You're always the last step.

## What it knows about your writing

The AI has been taught your writing style. It knows:
- You write in lowercase titles
- You never use em dashes
- You're sardonic but not mean
- You always admit your own hypocrisy before criticizing others
- You end with nuance ("it depends"), not simple answers
- You use parenthetical asides (like this one)
- You break grammar rules on purpose for emphasis

It also has 3 of your real articles saved in `reference/` so it can match your rhythm and tone.

## The pipeline (what happens each cycle)

```
Monday:  Planner creates tasks for the week
         |
         v
Step 1:  RESEARCH - AI scans travel news, ethical tourism stories,
         niche destinations, trending topics
         |
         v
Step 2:  DRAFT - AI writes a first draft in your voice
         |
         v
Step 3:  REVIEW - AI checks the draft against your quality standards
         |
         v
Step 4:  YOU - read it, add your stories, fix the voice, publish
```

## FAQ

**Can I just ignore this and write normally?**
Yes! This is a helper, not a replacement. If you want to write something yourself, just do it. The factory runs in the background.

**What if the AI writes something bad?**
Delete it or ignore it. Nothing gets published without you. The drafts are suggestions, not commands.

**What if I want it to stop?**
Tell David. He can pause the whole thing in 10 seconds.

**Can I see what the AI has been doing?**
Yes! Check the [dashboard](https://david0723.github.io/fialka-factory/) or look at the [Issues tab](https://github.com/david0723/fialka-factory/issues?q=is%3Aissue) to see all past tasks.

**How do I ask for something specific?**
Create an issue with the `operator` label. Write in plain English. Examples above.

**Does this cost money?**
Nope. David set it up on his infrastructure. You just use it.

---

*Built with [Depot](https://github.com/david0723/depot-template) - David's AI agent factory framework.*
