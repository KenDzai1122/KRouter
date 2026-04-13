<div align="center">
  <img src="./assets/banner.png" alt="KRouter banner" width="920" />

  # KRouter

  **Bilingual setup guides for Codex on KenDev-API**

  [![Guide](https://img.shields.io/badge/Guide-Vietnamese%20%2B%20English-0f172a?style=for-the-badge)](./README.vi.md)
  [![Codex](https://img.shields.io/badge/Codex-KenDev--API-2563eb?style=for-the-badge)](./README.en.md)
  [![Status](https://img.shields.io/badge/Docs-Ready-16a34a?style=for-the-badge)](./README.en.md)
</div>

## Overview

KRouter provides a clean Codex setup guide for KenDev-API users.
This repository now separates the documentation into:

- [Vietnamese Guide](./README.vi.md)
- [English Guide](./README.en.md)

## Quick Access

<table>
  <tr>
    <td align="center" width="50%">
      <h3>Tiếng Việt</h3>
      <p>Hướng dẫn cài đặt, cấu hình <code>config.toml</code>, <code>auth.json</code>, đổi model, và lưu ý tránh lỗi.</p>
      <p><a href="./README.vi.md"><strong>Mở README.vi.md</strong></a></p>
    </td>
    <td align="center" width="50%">
      <h3>English</h3>
      <p>Complete setup instructions for <code>config.toml</code>, <code>auth.json</code>, model switching, and safety notes.</p>
      <p><a href="./README.en.md"><strong>Open README.en.md</strong></a></p>
    </td>
  </tr>
</table>

## Supported Tools

<table>
  <tr>
    <td align="center" width="16%">
      <img src="https://cdn.simpleicons.org/visualstudiocode/007ACC" alt="VS Code" width="56" /><br />
      <strong>VS Code</strong><br />
      <sub>Main editor setup</sub>
    </td>
    <td align="center" width="16%">
      <img src="./assets/codex.png" alt="Codex App" width="56" /><br />
      <strong>Codex App</strong><br />
      <sub>Desktop workflow</sub>
    </td>
    <td align="center" width="16%">
      <img src="./assets/codex.png" alt="Codex CLI" width="56" /><br />
      <strong>Codex CLI</strong><br />
      <sub>Terminal usage</sub>
    </td>
    <td align="center" width="16%">
      <img src="./assets/cursor.png" alt="Cursor" width="56" /><br />
      <strong>Cursor</strong><br />
      <sub>AI IDE workflow</sub>
    </td>
    <td align="center" width="16%">
      <img src="./assets/opencode.png" alt="OpenCode" width="56" /><br />
      <strong>OpenCode</strong><br />
      <sub>Open coding agent</sub>
    </td>
    <td align="center" width="16%">
      <img src="./assets/openclaw.png" alt="OpenClaw" width="56" /><br />
      <strong>OpenClaw</strong><br />
      <sub>Multi-agent client</sub>
    </td>
  </tr>
  <tr>
    <td align="center" width="16%">
      <img src="./assets/claude.png" alt="Claude Code" width="56" /><br />
      <strong>Claude Code</strong><br />
      <sub>Anthropic tooling</sub>
    </td>
    <td align="center" width="16%">
      <img src="./assets/gemini-cli.png" alt="Gemini CLI" width="56" /><br />
      <strong>Gemini CLI</strong><br />
      <sub>Google CLI flow</sub>
    </td>
    <td align="center" width="16%">
      <img src="./assets/codex.png" alt="KenDev API" width="56" /><br />
      <strong>KenDev-API</strong><br />
      <sub>Model provider</sub>
    </td>
    <td align="center" width="16%">
      <img src="https://cdn.simpleicons.org/json/000000" alt="config.toml" width="56" /><br />
      <strong>config.toml</strong><br />
      <sub>Core config</sub>
    </td>
    <td align="center" width="16%">
      <img src="https://cdn.simpleicons.org/openai/412991" alt="OpenAI Key" width="56" /><br />
      <strong>auth.json</strong><br />
      <sub>API key auth</sub>
    </td>
    <td align="center" width="16%">
      <img src="https://cdn.simpleicons.org/markdown/000000" alt="Docs" width="56" /><br />
      <strong>Docs</strong><br />
      <sub>VN + EN guides</sub>
    </td>
  </tr>
</table>

## What The Guides Cover

- How to set `model`, `model_provider`, and `sandbox_mode` in `config.toml`
- How to configure `auth.json` with your API key
- How to switch Codex models safely using `Available KenDev-API models`
- Why you should not change models directly in the chat bar
- Notes about suffixes like `-xhigh`, `-high`, and `-medium`

## Recommended Reading Order

1. Open the guide in your preferred language.
2. Copy the `config.toml` template.
3. Fill in `auth.json`.
4. Restart VS Code after saving the files.

## Language Files

- [README.vi.md](./README.vi.md)
- [README.en.md](./README.en.md)
