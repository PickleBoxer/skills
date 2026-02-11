# Skills Repository

## Install a Skill

```bash
npx skills add PickleBoxer/skills
```

### Source Formats

```bash
# GitHub shorthand (owner/repo)
npx skills add PickleBoxer/skills

# Full GitHub URL
npx skills add https://github.com/PickleBoxer/skills

# Local path
npx skills add ./my-local-skills
```

### Options

| Option                    | Description                                                                                                                                        |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| `-g, --global`            | Install to user directory instead of project                                                                                                       |
| `-a, --agent <agents...>` | <!-- agent-names:start -->Target specific agents (e.g., `claude-code`, `codex`). See [Available Agents](#available-agents)<!-- agent-names:end -->                  |
| `-s, --skill <skills...>` | Install specific skills by name (use `'*'` for all skills)                                                                                         |
| `-l, --list`              | List available skills without installing                                                                                                           |
| `-y, --yes`               | Skip all confirmation prompts                                                                                                                      |
| `--all`                   | Install all skills to all agents without prompts                                                                                                   |

### Examples

```bash
# List skills in a repository
npx skills add PickleBoxer/skills --list

# Install specific skills
npx skills add PickleBoxer/skills --skill frontend-design --skill skill-creator

# Install to specific agents
npx skills add PickleBoxer/skills -a claude-code -a opencode

# Non-interactive installation (CI/CD friendly)
npx skills add PickleBoxer/skills --skill frontend-design -g -a claude-code -y

# Install all skills from a repo to all agents
npx skills add PickleBoxer/skills --all

# Install all skills to specific agents
npx skills add PickleBoxer/skills --skill '*' -a claude-code

# Install specific skills to all agents
npx skills add PickleBoxer/skills --agent '*' --skill frontend-design
```

Read more:
[vercel-labs/skills](https://github.com/vercel-labs/skills)
[skills.sh](https://skills.sh/)