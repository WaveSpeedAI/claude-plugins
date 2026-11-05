<div align="center">
  <a href="https://wavespeed.ai" target="_blank">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="assets/wavespeed-logo-dark.svg">
      <img src="assets/wavespeed-logo-light.svg" alt="WaveSpeed" width="342" height="48"/>
    </picture>
  </a>
</div>

# WaveSpeed plugins for Claude Code

Official [WaveSpeed](https://wavespeed.ai) plugin marketplace for Claude Code.

## Install

```
/plugin marketplace add WaveSpeedAI/claude-plugins
/plugin install wavespeed@wavespeed
```

## Plugins

### wavespeed

Generate and edit AI media — image, video, audio, 3D — on the WaveSpeed platform, through the hosted WaveSpeed MCP server and the open-source [`@wavespeed/cli`](https://github.com/WaveSpeedAI/wavespeed-cli). Every model on the platform is one `wavespeed run <model-id>` call; the skill teaches the agent the find → inspect → run pattern, `@path` local-file upload, and price checks before running.

The plugin brings two things:

- **The hosted WaveSpeed MCP server** (`https://api.wavespeed.ai/mcp`), with tools to generate, edit and extend images and videos, run any model, check prices and balance. Nothing to install: after the plugin is installed, run `/mcp`, pick `wavespeed` and approve the connection on the WaveSpeed page that opens (it creates an API key named `MCP · …` that you can delete on the [API Keys](https://wavespeed.ai/accesskey) page to disconnect). The hosted server cannot read files on your computer; pass public URLs, or use the CLI below for local files.
- **The `wavespeed` skill** for the open-source CLI, which also handles local files: requires `npm install -g @wavespeed/cli` and a WaveSpeed API key (`wavespeed login`).

Prefer the local MCP server instead? [`@wavespeed/mcp`](https://github.com/WaveSpeedAI/mcp-server): `claude mcp add wavespeed -- npx -y @wavespeed/mcp@latest`.

## Also works in GitHub Copilot CLI, Factory Droid and Qwen Code

All three read this marketplace directly, no separate package:

```
copilot plugin marketplace add WaveSpeedAI/claude-plugins      # then /plugin install wavespeed@wavespeed
droid plugin marketplace add WaveSpeedAI/claude-plugins        # then droid plugin install wavespeed@wavespeed --scope user
qwen extensions install WaveSpeedAI/claude-plugins:wavespeed
```

## Same skill, other agents

- Claude Code / Cursor / Codex without plugins: `wavespeed skill install`
- Codex: [codex-plugins](https://github.com/WaveSpeedAI/codex-plugins)
- OpenCode: [wavespeed-opencode](https://github.com/WaveSpeedAI/wavespeed-opencode)
- DeepSeek Harness: [wavespeed-dsh-skill](https://github.com/WaveSpeedAI/wavespeed-dsh-skill)
- Gemini CLI: [wavespeed-gemini-extension](https://github.com/WaveSpeedAI/wavespeed-gemini-extension)
- Kimi Code CLI: [wavespeed-kimi-plugin](https://github.com/WaveSpeedAI/wavespeed-kimi-plugin) — `/plugins install https://github.com/WaveSpeedAI/wavespeed-kimi-plugin` (also reads `.claude/skills/` directly, so `wavespeed skill install` works as-is)

## License

[MIT](LICENSE)

---

**[WaveSpeed AI](https://wavespeed.ai/)** — AI image & video generation platform.
Try it in the browser: **[Image generator](https://wavespeed.ai/image-generator)** · **[Video generator](https://wavespeed.ai/video-generator)**
