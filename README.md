# Volumatic VIDYA Optimized for TradingView

© realanthonyc  
https://x.com/anthonycxc | https://www.tradingview.com/u/realanthonyc

Pine Script® v6

## Overview
Volumatic VIDYA Optimized builds on BigBeluga’s original script and extends it with adaptive trend logic, liquidity tracking, and contextual visuals. The goal is to highlight the current bias, show where liquidity sits, and quantify volume pressure without clutter or repaint-heavy tricks.

## What the script does
- **Adaptive VIDYA + ATR bands** that flip trend bias automatically (regular settings for higher TFs, sensitive set for intraday).
- **Liquidity zones** drawn from pivot highs/lows with dotted extensions, capped arrays, and volume markers when price taps the line.
- **Volume delta stats** showing total buy, sell, and % delta for the active trend on the latest bar.
- **Sideways filter & visuals** using KDJ(9,3); sideways zones fade the gradient, while shadow/label colors stay user controlled.
- **Huge Performance improvement** by rewriting many parts of the script. Limits lines/labels to prevent lag; uses safe array management and processes only recent bars.

## What’s on the chart
- Dotted VIDYA line + optional HL2 reference with gradient fill between them.
- Liquidity lines with circle/volume labels when they’re hit.
- Last-bar label summarizing Buy, Sell, and Delta volume.

## Alerts
1. `Trend Up` – trend flipped bullish.  
2. `Trend Down` – trend flipped bearish.  
3. `Trend Changed` – fires on any flip if you prefer one alert to route logic yourself.

## Changelog
Please refer to the release notes.
