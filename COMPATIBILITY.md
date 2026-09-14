# Compatibility / 兼容性

One SKILL.md, no scripts, no dependencies. 安装即用，无脚本依赖。

| Agent | Install | Notes |
|---|---|---|
| Claude Code | `npx skills add ChenneyZhuang/project-handoff` or clone to `~/.claude/skills/` | model-invoked via description triggers |
| Codex CLI | `npx skills add ChenneyZhuang/project-handoff` | same SKILL.md |
| Cursor | `npx skills add ChenneyZhuang/project-handoff` | loads per CLI mapping |
| OpenCode / Windsurf / Gemini CLI / Cline / AMP / GitHub Copilot | `npx skills add ChenneyZhuang/project-handoff` | 75+ agents via skills CLI |
| DSH | clone, `dsh plugin --profile <name> add link:<repo>` | `dsh.bundle` manifest included |
| Hermes | `cp -r` into `~/.hermes/profiles/<profile>/skills/project-handoff/` | verify with `hermes skills` |

Runtime needs: file read/write only. 运行时只要文件读写。
