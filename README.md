# TickSurfers plugins

Plugins that connect AI coding and chat assistants to [TickSurfers Chart](https://ticksurfers.com/chart/) through its hosted MCP server, so an assistant can write, validate, backtest, and save custom indicators and trading strategies for your account.

| Plugin | For | Folder |
| --- | --- | --- |
| TickSurfers Chart | Claude and Claude Code | [`plugins/ticksurfers-chart-claude`](plugins/ticksurfers-chart-claude) |
| TickSurfers Chart | Cursor | [`plugins/ticksurfers-chart-cursor`](plugins/ticksurfers-chart-cursor) |

Not using Claude or Cursor? The MCP server works with ChatGPT and any app that supports remote MCP servers with OAuth sign-in. Add `https://ticksurfers.com/api/chart/ai/mcp` and follow the per-app steps at https://ticksurfers.com/connect.

A free TickSurfers account can validate, list, and save studies. Backtesting requires Pro. Backtests are historical simulations and do not establish future returns; nothing here is financial advice.

The plugin files in this repository are MIT licensed. The TickSurfers service is provided under the [terms of service](https://ticksurfers.com/legal/terms).
