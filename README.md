# MacroAgent Marketplace

Claude plugin marketplace for MacroAgent trading intelligence tools.

## Installation

### Step 0 — Install uv (if not already installed)

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

`uv` is required to run the MCP server. Restart your terminal after installing.

### Step 1 — Add this marketplace to Claude

```bash
claude plugin marketplace add MacroAgent/macroagent-marketplace
```

### Step 2 — Install the BTC report plugin

```bash
claude plugin install btc-orderflow-mcp@macroagent-marketplace
```

### Step 3 — Set your API key (persistent)

```bash
echo 'export BTC_MCP_API_URL="https://macroagent.ai"' >> ~/.zshrc
echo 'export BTC_MCP_API_KEY="your-api-key-here"' >> ~/.zshrc
source ~/.zshrc
```

> Bash users: replace `~/.zshrc` with `~/.bashrc`.

Then restart Claude.

### Step 4 — Use it

Type `/btc-orderflow-mcp:btc-report` in any Claude session, or simply ask:

> "What's the current BTC market condition?"

Claude will automatically invoke the skill.

## Available Plugins

| Plugin | Description |
|--------|-------------|
| `btc-orderflow-mcp` | Real-time BTC order flow analysis — hourly AI reports |

## Get an API Key

Contact [@trader_jessepan](https://t.me/trader_jessepan) on Telegram.
