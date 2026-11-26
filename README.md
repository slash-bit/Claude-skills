# Claude Skills

Claude Code skills marketplace by slash-bit.

## Install

```
claude plugin marketplace add slash-bit/claude-skills
claude plugin install slash-bit-skills@slash-bit
```

To turn it on for every session in a project, commit this to the project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "slash-bit": { "source": { "source": "github", "repo": "slash-bit/claude-skills" } }
  },
  "enabledPlugins": { "slash-bit-skills@slash-bit": true }
}
```

## Skills

| Skill | What it does |
|---|---|
| `/add-issue` | Asks which repository, bug or feature, description, goal and definition of done, then drafts the issue, shows it to you and files it once you approve. New issues are labelled `bug`/`enhancement` + `needs-triage` so they line up with `/triage` from [mattpocock/skills](https://github.com/mattpocock/skills). |
