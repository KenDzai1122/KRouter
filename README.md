## Hướng Dẫn Tiếng Việt

### Bước 1: Cấu hình `config.toml`

Trên Windows, truy cập vào:
`C:\Users\<tên thư mục người dùng>\.codex`

Tìm file `config.toml`, mở file này để chỉnh sửa.

Xóa toàn bộ nội dung cũ và dán cấu hình bên dưới, sau đó lưu lại:

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

### Bước 2: Cấu hình `auth.json`

Truy cập:
`C:\Users\<tên thư mục người dùng>\.codex`

Tìm file `auth.json`, xóa toàn bộ nội dung cũ và dán nội dung sau:

```json
{
  "auth_mode": "apikey",
  "OPENAI_API_KEY": "<your key>"
}
```

Lưu file lại.

### Hướng dẫn thay đổi model và mode của Codex

Muốn thay đổi model, vào `Settings` rồi mở `Config` để mở file `config.toml`.

Tại đây, copy một model trong danh sách `Available KenDev-API models` và thay vào dòng:

```toml
model = "..."
```

Các model có hậu tố `-xhigh`, `-high`, `-medium` là các model đã kèm sẵn mode tương ứng.

Với các model này, không cần và không nên đổi mode trong thanh chat với agent.

Lưu ý quan trọng: để tránh lỗi, tuyệt đối không thay hoặc chọn model ở thanh chat.

### Ghi chú

- Bạn có thể bị mất các cuộc trò chuyện cũ.
- Mở `VS Code -> Extensions`, cài `Codex`, và bảo đảm bạn đang dùng phiên bản mới nhất trước khi cấu hình.
- Sau khi cấu hình xong, hãy khởi động lại VS Code. Nếu giao diện hiển thị đúng như mong đợi thì cấu hình đã hoạt động.

### Giới hạn

- Hiện tại subagent chưa hoạt động, nên công cụ chỉ chạy độc lập.
- Nếu muốn đổi model, hãy sửa dòng này trong `config.toml`:

```toml
model = "cx/gpt-5.4-xhigh"
```

### Các model hỗ trợ tốt

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

## English Guide

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

### How to change the Codex model and mode

To change the model, open `Settings`, then open `Config` to edit the `config.toml` file.

Copy one of the models listed under `Available KenDev-API models` and replace this line:

```toml
model = "..."
```

Models with suffixes like `-xhigh`, `-high`, and `-medium` already include their intended mode.

For those models, you should not change the mode in the chat bar with the agent.

Important: to avoid errors, do not change or select models from the chat bar.

### Notes

- You may lose previous chat sessions.
- Open `VS Code -> Extensions`, install `Codex`, and make sure you are using the latest version before configuring it.
- After setup is complete, restart VS Code. If the interface looks correct, the configuration is working.

### Limitations

- Subagents are currently not working, so it runs independently only.
- To change the model, edit this line in `config.toml`:

```toml
model = "cx/gpt-5.4-xhigh"
```

### Supported models

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
