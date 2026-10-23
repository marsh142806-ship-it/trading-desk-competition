# Trading Desk 15-Day Capital Competition

Two systems compete with ~$100 each for 15 days. Winner (higher total portfolio value) stays; loser is shut down.

## Systems

### System 1 – Previous Multi-Agent Desk
- Portfolio: `System1-Previous-Desk` (`04522c02-2964-4b7a-9503-17451b4a522a`)
- Starting capital: ~$100.63 (ZEC + USDC/USD)
- Style: Classic 6-agent pipeline (Scout / News / Chart / Skeptic / Risk / Gatekeeper)
- Automations: `System1-Previous-Desk :00` (and :30 when available)

### System 2 – Pure NautilusTrader-inspired
- Portfolio: `System2-Nautilus-MultiBot` (`07bf3122-aa33-4ec7-9d3f-77e63111a7e5`)
- Starting capital: exactly $100 USDC
- Style: Direct application of NautilusTrader open-source strategies (no previous multi-bot agents):
  - EMA crossover (trend following)
  - Bollinger Bands + RSI (mean reversion)
  - Order book imbalance / grid ideas when relevant
- Automations: `System2-Nautilus :00` (and :30 when available)

## Shared Core Rules (updated)
- ALWAYS BUY LOW AND SELL HIGH
- Trades up to $50 notional at once allowed when clear profit potential exists
- Stop-loss only if recovery looks unlikely (no mandatory tight exit-on-any-adverse-move)
- Compound all profits inside the system (no banking out)
- Free to trade any crypto or stocks/ETFs
- 15-day deathmatch starting ~22–23 Oct 2026
- Report after 8 days (after market close)

## Schedule Goal
Each system should have:
- One automation at :00 of every hour (all day)
- One automation at :30 of every hour (all day)
Total 4 automations.

## Source Inspiration
NautilusTrader: https://github.com/nautechsystems/nautilus_trader

Not financial advice. Live trading on Coinbase via Grok automations.
