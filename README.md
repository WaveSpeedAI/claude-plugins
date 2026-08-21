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

Generate and edit AI media — image, video, audio, 3D — through the WaveSpeed platform via the open-source [`@wavespeed/cli`](https://github.com/WaveSpeedAI/wavespeed-cli). Every model on the platform is one `wavespeed run <model-id>` call; the skill teaches the agent the find → inspect → run pattern, `@path` local-file upload, and price checks before running.

Requires the CLI (`npm install -g @wavespeed/cli`) and a WaveSpeed API key (`wavespeed login`).

Prefer an MCP server over a CLI skill? Use [`@wavespeed/mcp`](https://github.com/WaveSpeedAI/mcp-server) instead: `claude mcp add wavespeed -- npx -y @wavespeed/mcp`.

## Same skill, other agents

- Claude Code / Cursor / Codex without plugins: `wavespeed skill install`
- OpenCode: loads the installed skill as-is
- DeepSeek Harness: [wavespeed-dsh-skill](https://github.com/WaveSpeedAI/wavespeed-dsh-skill)
- Gemini CLI: [wavespeed-gemini-extension](https://github.com/WaveSpeedAI/wavespeed-gemini-extension)

## License

[MIT](LICENSE)

---

**[WaveSpeed AI](https://wavespeed.ai/)** — AI image & video generation platform.
Try it in the browser: **[Image generator](https://wavespeed.ai/image-generator)** · **[Video generator](https://wavespeed.ai/video-generator)**
