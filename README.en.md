# English Guide

<div align="center">
  <img src="./assets/banner.png" alt="KRouter banner" width="920" />
</div>

## Quick Setup

### Step 1: Configure `config.toml`

On Windows, go to:
`C:\Users\<your user folder name>\.codex`

Find the file `config.toml` and open it for editing.

Delete all existing content and paste the config below, then save:

```toml
model = "cx/gpt-5.4-xhigh"
model_provider = "KenDev-API"
sandbox_mode = "danger-full-access"

# Available KenDev-API models:
# cx/gpt-5.4
# cx/gpt-5.4-xhigh
# cx/gpt-5.4-high
# cx/gpt-5.3-codex
# cx/gpt-5.3-codex-xhigh
# cx/gpt-5.3-codex-high
# cx/gpt-5.3-codex-low
# cx/gpt-5.3-codex-none
# cx/gpt-5.3-codex-spark
# cx/gpt-5.2-codex
# cx/gpt-5.2
# cx/gpt-5.1-codex-mini
# cx/gpt-5.1-codex-mini-high
# cx/gpt-5.1-codex-max
# cx/gpt-5.1-codex
# cx/gpt-5.1
# cx/gpt-5-codex
# cx/gpt-5-codex-mini

[model_providers.KenDev-API]
name = "KenDev-API"
base_url = "http://14.225.255.58:20128/v1"
wire_api = "responses"

[agents.subagent]
model = "cx/gpt-5.3-codex-xhigh"

[windows]
sandbox = "unelevated"
```

### Step 2: Configure `auth.json`

Go to:
`C:\Users\<your user folder name>\.codex`

Find the file `auth.json`, delete everything inside it, and paste:

```json
{
  "auth_mode": "apikey",
  "OPENAI_API_KEY": "<your key>"
}
```

Save the file.

## How to change the Codex model and mode

To change the model, open `Settings`, then open `Config` to edit the `config.toml` file.

Copy one of the models listed under `Available KenDev-API models` and replace this line:

```toml
model = "..."
```

Models with suffixes like `-xhigh`, `-high`, and `-medium` already include their intended mode.

For those models, you should not change the mode in the chat bar with the agent.

Important: to avoid errors, do not change or select models from the chat bar.

## Notes

- You may lose previous chat sessions.
- Open `VS Code -> Extensions`, install `Codex`, and make sure you are using the latest version before configuring it.
- Restart VS Code after finishing the setup.

## Limitations

- Subagents are currently not working, so it runs independently only.
- To change the model, edit this line in `config.toml`:

```toml
model = "cx/gpt-5.4-xhigh"
```

## Supported models

```txt
# cx/gpt-5.4
# cx/gpt-5.4-xhigh
# cx/gpt-5.4-high
# cx/gpt-5.3-codex
# cx/gpt-5.3-codex-xhigh
# cx/gpt-5.3-codex-high
# cx/gpt-5.3-codex-low
# cx/gpt-5.3-codex-none
# cx/gpt-5.3-codex-spark
# cx/gpt-5.2-codex
# cx/gpt-5.2
# cx/gpt-5.1-codex-mini
# cx/gpt-5.1-codex-mini-high
# cx/gpt-5.1-codex-max
# cx/gpt-5.1-codex
# cx/gpt-5.1
# cx/gpt-5-codex
# cx/gpt-5-codex-mini
```

## Navigation

- [Back to main page](./README.md)
- [Open the Vietnamese guide](./README.vi.md)

