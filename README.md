# Options Strategy Reference Table

| Category | Strategy | Construction | Risk Profile | Market View | Use Case | Example (AAPL @ $170) | Options Price Breakdown |
|:--------:|:--------:|:------------:|:------------:|:-----------:|:--------:|:---------------------|:----------------------|
| **2-LEG SPREADS** | | | | | | | |
| | Vertical Call | Long + Short Call (diff strikes) | Limited | Bullish | Directional trade with defined risk | Buy 170C, Sell 175C for $2.50 net debit | Buy 170C @ $5.00 - Sell 175C @ $2.50 = $2.50 debit (ITM costs more than OTM) |
| | Vertical Put | Long + Short Put (diff strikes) | Limited | Bearish | Directional trade with defined risk | Buy 170P, Sell 165P for $2.20 net debit | Buy 170P @ $5.00 - Sell 165P @ $2.80 = $2.20 debit (ATM costs more than OTM) |
| | Calendar Call | Long + Short Call (diff exp) | Limited | Neutral-Bullish | Time decay exploitation | Buy Mar 170C, Sell Feb 170C for $1.80 net debit | Buy Mar 170C @ $5.50 - Sell Feb 170C @ $3.70 = $1.80 debit (Longer term costs more) |
| | Calendar Put | Long + Short Put (diff exp) | Limited | Neutral-Bearish | Time decay exploitation | Buy Mar 170P, Sell Feb 170P for $1.60 net debit | Buy Mar 170P @ $5.30 - Sell Feb 170P @ $3.70 = $1.60 debit (Time value difference) |
| | Diagonal Call | Long + Short Call (diff strikes/exp) | Limited | Mod. Bullish | Directional with time decay | Buy Mar 170C, Sell Feb 175C for $2.70 net debit | Buy Mar 170C @ $5.50 - Sell Feb 175C @ $2.80 = $2.70 debit (Strike + time spread) |
| | Diagonal Put | Long + Short Put (diff strikes/exp) | Limited | Mod. Bearish | Directional with time decay | Buy Mar 170P, Sell Feb 165P for $2.40 net debit | Buy Mar 170P @ $5.30 - Sell Feb 165P @ $2.90 = $2.40 debit (Strike + time spread) |
| | Ratio Call | 1 Long : Multiple Short Calls | Unlimited | Neutral-Bullish | Premium collection | Buy 1 170C, Sell 2 175C for $0.50 net credit | Buy 170C @ $5.00 - (2 × Sell 175C @ $2.75) = $0.50 credit (2:1 ratio) |
| | Ratio Put | 1 Long : Multiple Short Puts | Unlimited | Neutral-Bearish | Premium collection | Buy 1 170P, Sell 2 165P for $0.40 net credit | Buy 170P @ $5.00 - (2 × Sell 165P @ $2.70) = $0.40 credit (2:1 ratio) |
| **3-LEG SPREADS** | | | | | | | |
| | Butterfly Call | Buy-Sell-Sell-Buy Calls | Limited | Neutral | Precise price targeting | Buy 165C, Sell 2 170C, Buy 175C for $1.50 net debit | Buy 165C @ $8.00 - (2 × Sell 170C @ $5.00) + Buy 175C @ $3.50 = $1.50 debit |
| | Butterfly Put | Buy-Sell-Sell-Buy Puts | Limited | Neutral | Precise price targeting | Buy 165P, Sell 2 170P, Buy 175P for $1.40 net debit | Buy 165P @ $7.80 - (2 × Sell 170P @ $5.00) + Buy 175P @ $3.60 = $1.40 debit |
| | Custom 3 Leg | Varies | Variable | Varies | Custom risk/reward setup | Buy 170C, Sell 175C, Sell 165P for net credit | Structure varies based on strategy goals |
| **4-LEG SPREADS** | | | | | | | |
| | Condor Call | 4 Calls (diff strikes) | Limited | Neutral | Range-bound trading | Buy 165C, Sell 170C, Sell 175C, Buy 180C for $2.00 net debit | Buy 165C @ $8.00 - Sell 170C @ $5.00 - Sell 175C @ $2.50 + Buy 180C @ $1.50 = $2.00 debit |
| | Condor Put | 4 Puts (diff strikes) | Limited | Neutral | Range-bound trading | Buy 165P, Sell 170P, Sell 175P, Buy 180P for $1.90 net debit | Buy 165P @ $7.80 - Sell 170P @ $5.00 - Sell 175P @ $2.40 + Buy 180P @ $1.50 = $1.90 debit |
| | Iron Condor | Put Spread + Call Spread | Limited | Neutral | Premium collection | Sell 165P/170P, Sell 175C/180C for $2.50 net credit | (Sell 170P - Buy 165P) @ $2.00 + (Sell 175C - Buy 180C) @ $0.50 = $2.50 credit |
| **COMBINATIONS** | | | | | | | |
| | Covered Call | Long Stock + Short Call | Limited Upside | Slightly Bullish | Income generation | Buy 100 shares @ $170, Sell 175C for $3.50 | Stock cost $170 - Call premium $3.50 = $166.50 net debit per share |
| | Covered Put | Short Stock + Short Put | Limited Upside | Slightly Bearish | Income generation | Short 100 shares @ $170, Sell 165P for $3.00 | Short stock @ $170 + Put premium $3.00 = $173 net credit per share |
| | Protective Call | Long Stock + Long Call | Limited | Bullish + Protection | Portfolio protection | Long 100 shares @ $170, Buy 175C for $2.50 | Stock cost $170 + Call cost $2.50 = $172.50 net debit per share |
| | Protective Put | Long Stock + Long Put | Limited | Bearish + Protection | Downside protection | Long 100 shares @ $170, Buy 165P for $2.20 | Stock cost $170 + Put cost $2.20 = $172.20 net debit per share |
| | Straddle | Long Call + Long Put (same strike) | Limited | Volatile | Large move expected | Buy 170C and 170P for $10.00 net debit | Buy 170C @ $5.00 + Buy 170P @ $5.00 = $10.00 debit (ATM options) |
| | Strangle | Long Call + Long Put (diff strikes) | Limited | Volatile | Large move expected | Buy 175C and 165P for $5.50 net debit | Buy 175C @ $2.50 + Buy 165P @ $3.00 = $5.50 debit (OTM options) |

Key Price Factors:
- ITM (In-The-Money) options cost more than OTM (Out-of-The-Money)
- Longer expiration dates cost more than shorter ones
- ATM (At-The-Money) options have highest time value
- Net Debit = You pay to open position
- Net Credit = You receive money to open position
- All prices are hypothetical examples using AAPL @ $170
