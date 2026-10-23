# Trading Desk 15-Day Capital Competition

Two multi-bot systems compete with ~$100 each for 15 days. Winner (higher total portfolio value) stays; loser is shut down.

## Systems

### System 1 – Previous Multi-Agent Desk
- Portfolio: `System1-Previous-Desk` (`04522c02-2964-4b7a-9503-17451b4a522a`)
- Starting capital: ~$100.63 (ZEC + USDC/USD)
- Style: Classic 6-agent pipeline (Scout / News / Chart / Skeptic / Risk / Gatekeeper)
- Automation: `System1-Previous-Desk (Competition)` (taskId: cc8ef5f7-de93-4d05-8dce-32940a037648)

### System 2 – Nautilus-inspired MultiBot
- Portfolio: `System2-Nautilus-MultiBot` (`07bf3122-aa33-4ec7-9d3f-77e63111a7e5`)
- Starting capital: exactly $100 USDC
- Style: Same 6-agent structure + primary signals from NautilusTrader open-source examples:
  - EMA crossover (trend following)
  - Bollinger Bands + RSI (mean reversion)
  - Optional grid / order-book ideas
- Automation: `System2-Nautilus-MultiBot (Competition)` (taskId: 32417ec8-9ca1-4d46-8043-c40bc0d208f4)

## Shared Rules
- Tight risk: prefer exit on any adverse move; stop only if recovery looks unlikely
- Position size 1–3% of current portfolio value
- Compound all profits inside the system (no banking out)
- Free to trade any crypto or stocks/ETFs
- 15-day deathmatch starting ~22–23 Oct 2026

## Old Automations
Previous Trading Desk Hourly and :30 Offset have been paused so they do not interfere.

## Source Inspiration
NautilusTrader: https://github.com/nautechsystems/nautilus_trader  
(EMA cross, BB+RSI, etc.)

Not financial advice. Live trading on Coinbase via Grok automations.
