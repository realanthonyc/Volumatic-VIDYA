# Volumatic VIDYA: Trend & Liquidity for TradingView

© realanthonyc  
https://x.com/anthonycxc | https://www.tradingview.com/u/realanthonyc

Pine Script® v6

## Overview
Volumatic VIDYA Trend & Liquidity builds on BigBeluga’s original script and extends it with adaptive trend logic, liquidity tracking, and contextual visuals. The goal is to highlight the current bias, show where liquidity sits, and quantify volume pressure without clutter or repaint-heavy tricks.

## What the script does
- **Adaptive VIDYA + ATR bands** that flip trend bias automatically, with dual configuration sets — Regular (for daily & higher timeframes) and Sensitive (for intraday) — providing smoother trends on higher TFs and faster reactions on lower TFs.
- **Timeframe-aware liquidity zones** drawn from pivot highs/lows (shorter pivots below 1h) with dotted extensions, capped arrays, and markers when price taps the line.
- **Configurable volume stats** showing total buy, sell, and % delta for the active trend on the latest bar, reset on flips and calculated by your chosen method (3-Bars, Average, Pivot Bar, or Pivot Window).
- **Huge Performance improvement** by rewriting many parts of the script. Limits lines/labels to prevent lag; uses safe array management and processes only recent bars.

## What's on the chart
- Dotted VIDYA line + optional HL2 reference with gradient fill between them.
- Liquidity lines with circle markers when they’re hit; optional volume labels if enabled.
- Last-bar label summarizing Buy, Sell, and Delta volume.

## Alerts
1. `Trend Up` – trend flipped bullish.  
2. `Trend Down` – trend flipped bearish.  
3. `Trend Changed` – fires on any flip if you prefer one alert to route logic yourself.

Alerts confirm on the bar after a flip (state check uses the prior bar).

## Changelog
Please refer to the release notes.
