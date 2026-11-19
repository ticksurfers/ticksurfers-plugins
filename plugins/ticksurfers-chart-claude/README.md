# TickSurfers Chart plugin for Claude

Create, validate, backtest, and save custom indicators and trading strategies for TickSurfers Chart from Claude and Claude Code.

## Install

In Claude Code: `/plugin marketplace add ticksurfers/ticksurfers-plugins`, then `/plugin install ticksurfers-chart@ticksurfers-plugins`. Slash commands: `/ticksurfers-chart:new-indicator` and `/ticksurfers-chart:new-strategy`.

## What it does

Lets your AI assistant write, check, backtest, and save custom indicators and trading strategies for [TickSurfers Chart](https://ticksurfers.com/chart/), using real chart functions instead of guessing.

- Reads the current coding guide and technical-analysis catalog before writing code.
- Validates indicator and strategy code and reports errors and warnings.
- Backtests strategies on historical data (requires TickSurfers Pro).
- Lists your saved indicators and strategies and saves new ones as personal studies in your Chart account.

## Tools

The plugin connects your assistant to TickSurfers' hosted MCP server. The assistant chooses the tools for you:

| Tool | Purpose | Plan |
| --- | --- | --- |
| `chart_oracle_health` | Check the service responds and which capabilities are available | Free |
| `chart_study_protocol` | Read the coding guide and examples | Free |
| `chart_ta_catalog` | Search built-in technical-analysis functions | Free |
| `chart_validate_study` | Run code on sample bars and report errors and warnings | Free |
| `chart_backtest_strategy` | Backtest a strategy on historical bars | Pro |
| `chart_list_studies` | List the names of your saved studies | Free |
| `chart_save_study` | Validate and save a study to your account | Free |

## Example prompts

- "Create a 14-period RSI indicator with 30 and 70 levels for TickSurfers Chart. Validate it and show me the code."
- "Build a strategy that buys SPY when the 10-period moving average crosses above the 20-period average and exits on the cross below. Backtest it on 500 daily bars with $100,000 starting capital."
- "Save that indicator to my TickSurfers account as My RSI."

## Accounts and sign-in

A [free TickSurfers account](https://ticksurfers.com/free) (email only, no card) can validate, list, and save studies. Backtesting requires [Pro](https://ticksurfers.com/pricing). On first use your AI app opens a TickSurfers page in your browser: sign in and choose Approve. Your password is never shared with the AI app, and the plugin contains no credentials. You can review or disconnect connected apps from the AI agents tab in your Chart account. Connections expire after 30 days.

## What it runs and connects to

The plugin contains no scripts, hooks, or local servers. It declares one remote MCP server at `https://ticksurfers.com/api/chart/ai/mcp` (Streamable HTTP, OAuth). TickSurfers receives only what your assistant sends in tool calls: indicator or strategy code, backtest settings, and the name and description of anything you save. See the [privacy policy](https://ticksurfers.com/legal/privacy) and [terms](https://ticksurfers.com/legal/terms).

## Limits and safety

- It cannot place trades, reach a brokerage account, delete your studies, or read other customers' private code.
- Nothing is saved unless you ask. Saved studies are private to you by default.
- Backtests are historical simulations and do not establish future returns. See the [risk disclosure](https://ticksurfers.com/legal/risk). Nothing here is financial advice.

## Help

Setup guide: https://ticksurfers.com/connect. Questions or problems: https://ticksurfers.com/contact. Licensed under MIT (plugin files only).
