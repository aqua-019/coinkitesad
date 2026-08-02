# COINKITE ($115792)

> 115,792,089,237,316,195,423,570,985,008,687,907,853,269,984,665,640,564,039,457,584,007,913,129,639,936

The number held. The firmware did not. A commemorative meme token on Solana, born in Mayhem Mode.

- **CA:** `FwxtoAzKjAT4KsL8XeoqM1FU3PmzWtiMFDBQ3jFepump`
- **Chart:** https://dexscreener.com/solana/cw959iwe22ev8rvfmxrkeqexowuoo8v4bhmpjkuebmvv
- **pump.fun:** https://pump.fun/coin/FwxtoAzKjAT4KsL8XeoqM1FU3PmzWtiMFDBQ3jFepump
- **Solscan:** https://solscan.io/token/FwxtoAzKjAT4KsL8XeoqM1FU3PmzWtiMFDBQ3jFepump

## Deploy

Vercel → Add New Project → Import this repo → Framework preset: **Other** → Deploy.
One static file, zero build step, zero config. Live data hydrates client-side from the
DexScreener API and public Solana RPC.

## Sections

- **Live market** — price, mcap/FDV, liquidity, 24h volume, buy/sell flow, 1h/6h/24h
  deltas, pool reserves, turnover, live on-chain supply, activity buckets, ticking pair
  age, a reconstructed trend sparkline, and the burn record (1B of 2B minted).
- **Swap console** — terminal-styled, computes quotes in-browser from live pool reserves
  (constant-product), estimates price impact, settles on Jupiter / pump.fun. No wallet
  connection, ever.
- **Liquidity pool** — the x·y=k hyperbola drawn from live reserves; drag the marker (or
  use the steppers / arrow keys) to simulate buys and sells and watch price impact.
- **Flow monitor** — live transaction feed with side (buy/sell), token, SOL and USD
  amounts parsed from each tx's balance deltas.
- **Entropy ceremony** — roll a 3D die powered by the browser CSPRNG; rolls stack into a
  grid and deterministically derive a demo recovery phrase. A novelty — never secure real
  funds with a phrase from a website.

Chart source is switchable (**GeckoTerminal** default, then DexScreener / Jupiter) in
case an embed is blocked.

### Incident data (`incident.json`)

The "Incident metrics" section is an ongoing situation. The counts (BTC relocated,
addresses swept, % unspent, as-of timestamp) load from `incident.json` so they can be
updated in a single small commit; the USD figure is computed live in the browser against
the Bitcoin spot price (Coinbase, CoinGecko fallback). Current values as of 2026-08-02:
1,367.05 BTC across 4,585 addresses (~$88.6M), three waves, 100% unspent. Edit
`incident.json` to refresh the headline numbers.

### Dice ceremony

The die uses the browser CSPRNG. Derivation is transparent and coordinated: every 4 rolls
map (base-6) to one word, shown as `[d][d][d][d] → word` in a ledger under the button and
mirrored in the phrase grid. 48 rolls → 12 words, 96 → 24. A novelty — never a real seed.

## Design

Built from the Design Variable Catalogue 3000 — Category 41 (*The Anthropic Reference
System*, D3001–D3075) plus the S-tier working set: ivory ground, one clay accent,
class-scoped theme inversion, named-line breakout grid, two-point clamp type scale,
four easing tokens, colour-only hovers, 0fr→1fr disclosures, hover-paused 48s number
belt, FOUC-guarded word reveal, scroll-reveal choreography, magnetic CTA, the pool
set-piece (D3058-family: draggable, pre-bloom gated, bounded steppers, bobbing hint,
giant serif landmark), copy-confirm morph, live-region announcements, reduced-motion
parity per component.

## Disclaimer

Unaffiliated parody / commemorative token. No relationship to Coinkite Inc., COLDCARD,
or any hardware wallet manufacturer. References to security events link to third-party
journalism. Not financial advice. The number is real, though.
