# Agentic Marketing Architecture Skills

A curated registry of practical Claude Skills for Marketing Architects building owned, systematic marketing infrastructure through the Agentic Marketing Architecture framework.

**Stop renting tools. Start building systems.**

---

## What Are Marketing Architecture Skills?

Marketing Architecture Skills are reusable, composable workflows that extend the Agentic Marketing Architecture framework. They're the building blocks you use to architect your own marketing systems—no lock-in, no subscriptions, no dependency on vendor roadmaps.

Unlike traditional automation templates (which hide how they work), skills are **transparent, modifiable, and permanently yours**. You understand every step. You control every decision. You own the infrastructure.

**In practical terms:** Skills teach Claude how to execute your specific workflows according to your brand standards and business requirements. They're the difference between using a tool (pushing buttons) and architecting a system (designing infrastructure).

---

## Skills Registry

### Strategic Planning
- **[youtube-strategy](./youtube-strategy/)** - Build YouTube channel strategy from market validation through execution using Paddy Galloway's proven framework. Includes TAM research, zero-competition keyword targeting, three-bucket content framework, phase-based publishing cadence, and packaging systems (titles, thumbnails, hooks, analytics)

---

## Getting Started

### Using Skills in Claude.ai

1. Click the skill icon (🧩) in your chat interface.
2. Add skills from the marketplace or upload custom skills.
3. Claude automatically activates relevant skills based on your task.

### Using Skills in Claude Code

1. Place the skill in `~/.config/claude-code/skills/`:
   ```bash
   mkdir -p ~/.config/claude-code/skills/
   cp -r skill-name ~/.config/claude-code/skills/
   ```

2. Verify skill metadata:
   ```bash
   head ~/.config/claude-code/skills/skill-name/SKILL.md
   ```

3. Start Claude Code:
   ```bash
   claude
   ```

4. The skill loads automatically and activates when relevant.

### Using Skills via API

Use the Claude Skills API to programmatically load and manage skills:

```python
import anthropic

client = anthropic.Anthropic(api_key="your-api-key")

response = client.messages.create(
    model="claude-3-5-sonnet-20241022",
    skills=["skill-id-here"],
    messages=[{"role": "user", "content": "Your prompt"}]
)
```

See the [Skills API documentation](https://docs.claude.com/en/api/skills-guide) for details.

---

## Philosophy

Most marketing tools want to make you dependent. They hide how they work. They charge more when you scale. They extract value from your success.

**We believe the opposite.**

When you adopt Marketing Architecture skills, you're not renting convenience—you're building capability. Every skill you create, modify, or master becomes part of your permanent infrastructure. The deeper you invest, the more valuable it becomes. Skills compound. Subscriptions extract.

This registry exists so that ambitious marketing strategists and agency owners can:

- **Own their infrastructure** - Build systems no vendor can lock you into
- **Learn from each other** - Contribute and benefit from collective knowledge
- **Maintain competitive advantage** - Proprietary workflows that improve with every use
- **Stay in the loop** - Keep human judgment and expertise architecturally central

**You're not users. You're builders.**

Build something better. Build something yours.

## Resources

### Official Documentation

- [Claude Skills Overview](https://www.anthropic.com/news/skills) - Official announcement and features
- [Skills User Guide](https://support.claude.com/en/articles/12512180-using-skills-in-claude) - How to use skills in Claude
- [Creating Custom Skills](https://support.claude.com/en/articles/12512198-creating-custom-skills) - Skill development guide
- [Skills API Documentation](https://docs.claude.com/en/api/skills-guide) - API integration guide
- [Agent Skills Blog Post](https://anthropic.com/engineering/equipping-agents-for-the-real-world-with-agent-skills) - Engineering deep dive

### Community Resources

- [Anthropic Skills Repository](https://github.com/anthropics/skills) - Official example skills
- [Claude Community](https://community.anthropic.com) - Discuss skills with other users
- [Skills Marketplace](https://claude.ai/marketplace) - Discover and share skills

### Inspiration & Use Cases

- [Lenny's Newsletter](https://www.lennysnewsletter.com/p/everyone-should-be-using-claude-code) - 50 ways people use Claude Code
- [Notion Skills](https://www.notion.so/notiondevs/Notion-Skills-for-Claude-28da4445d27180c7af1df7d8615723d0) - Notion integration skills