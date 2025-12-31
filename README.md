# XAUUSD Pro Suite

**Professional XAUUSD Trading Suite - 8-Layer Architecture**

![MT5 Indicator](https://img.shields.io/badge/Platform-MetaTrader%205-blue)  
![Language](https://img.shields.io/badge/Language-MQL5-orange)  
![Version](https://img.shields.io/badge/Version-1.00-green)  
![Optimized for](https://img.shields.io/badge/Optimized%20for-XAUUSD-gold)  
![Architecture](https://img.shields.io/badge/Architecture-8--Layer-purple)

## Overview

**XAUUSD Pro Suite** is an advanced, institutional-grade custom indicator designed **exclusively for Gold (XAUUSD)** trading.

It features an **8-layer architecture** with:

- Market regime detection (4 regimes)
- Self-adaptive parameters
- Edge decay awareness
- Strategy switching
- Non-repainting signals
- Premium real-time dashboard

The system automatically adapts to changing market conditions while protecting against overtrading during poor edge periods.

## 8-Layer Architecture

1. **Regime Detection** – Identifies 4 market states
2. **Strategy Selection** – Chooses optimal approach per regime
3. **Signal Generation** – Regime-specific entry logic
4. **Edge Metrics** – Tracks performance over last 20 signals
5. **Edge Status Evaluation** – Healthy / Weak / Disabled
6. **Rule-Based Adaptation** – Self-adjusts parameters
7. **Signal Gate** – Multiple filters (spread, volume, session)
8. **Dashboard & Visualization** – Real-time monitoring

## Market Regimes

| Regime               | Characteristics                     | Active Strategy       |
|----------------------|-------------------------------------|-----------------------|
| Strong Trend         | ADX > 28                            | Trend Pullback        |
| Range/Mean Reversion | ADX < 20                            | Range Fade            |
| High Volatility      | ATR spike + volume surge            | News Momentum Fade    |
| No Trade             | Low liquidity / high spread         | No signals            |

## Features

- **Fully Optimized for XAUUSD** with specific parameters
- **100% Non-Repainting** signals (confirmed on bar close)
- **Self-Adaptive System** – adjusts parameters based on performance
- **Edge Protection** – reduces/disables trading during drawdown
- **Multi-Strategy Engine** – switches automatically per regime
- **Advanced Filters**:
  - Spread filter
  - Volume filter
  - Session filter (no-trade hours)
  - News time avoidance
  - Cooldown period
- **Premium Dashboard** showing:
  - Current regime & strategy
  - Edge status & win rate
  - Next expected signal
  - Entry/SL/TP levels
  - Adaptation status
  - Session & spread info

## Visual Elements

| Element              | Symbol/Color                 | Meaning                                    |
|----------------------|------------------------------|--------------------------------------------|
| Buy Signal           | Lime upward arrow            | High-confidence long entry                 |
| Sell Signal          | Red downward arrow           | High-confidence short entry                |
| Trend Up             | DarkGreen markers            | Strong bullish trend confirmation          |
| Trend Down           | DarkRed markers              | Strong bearish trend confirmation          |

## Installation

1. Download `XAUUSD_Pro_Suite.mq5`
2. Open MetaTrader 5 → File → Open Data Folder
3. Navigate to `MQL5/Indicators/`
4. Copy the `.mq5` file into this folder
5. Restart MT5 or refresh Navigator
6. Apply to **XAUUSD** chart (recommended: H1, H4)

## Input Parameters

### Regime Settings
- ADX & ATR periods
- Trend/range thresholds
- ATR spike detection

### Strategy Settings
- EMA periods (Fast/Mid/Slow/Trend)
- RSI levels
- Stop loss & R:R multipliers

### Filter Settings
- Signal cooldown
- Max spread
- Volume minimum
- No-trade hours
- News filter minutes

### Adaptation Settings
- Enable self-adaptation
- Adaptation frequency
- Maximum change per adjustment
- Edge thresholds

### Alert & Dashboard Settings
- Alerts (popup/sound/push)
- Dashboard display options
- Colors and position

## Usage Recommendations

- **Primary instrument**: XAUUSD only
- **Best timeframes**: H1, H4
- Trust the **regime detection** – different strategies per market type
- Monitor **Edge Status**:
  - Healthy = full confidence
  - Weak = extra confirmation required
  - Disabled = system protects capital
- Let **adaptation** work – system learns from recent performance
- Use **dashboard** as primary monitoring tool

## Author

© Copyright by **M4DI~UciH4**  
GitHub: https://github.com/RizkyEvory

## Disclaimer

This indicator is provided for educational and personal use only.  
It is specifically optimized for XAUUSD — results may vary on other instruments.  
No guarantee of profitability. Trading involves significant risk.  
Use proper risk management.

---

**An intelligent, adaptive system that protects your edge while maximizing opportunities in Gold.** 🥇
