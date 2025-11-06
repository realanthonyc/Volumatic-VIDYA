# Volumatic-VIDYA
Volumatic VIDYA for TradingView

**Volumatic VIDYA Optimized** is a Pine Script v6 indicator that combines a Variable Index Dynamic Average (VIDYA) with ATR-based dynamic bands, pivot-based liquidity zones, and volume delta analysis to identify trend direction and high-probability support/resistance levels.

It is forked from the excellent work by BigBeluga: "Variable Index Dynamic Average" / "Volumatic VIDYA" indicator.

Key Features:
- Adaptive VIDYA Trend Line: Smooths price action based on momentum (CMO), switching between upper/lower ATR bands during uptrends/downtrends.
- Liquidity Zones: Detects swing pivots **using precise high/low prices for accurate support/resistance** and draws extendable dotted lines at key levels; short lines terminate with volume-labeled markers when price crosses.
- Volume Delta Tracking: Accumulates buy/sell volume per trend, displaying Buy/Sell volumes and % **Delta** on the last bar.
- Visual Enhancements: Trend-colored fill with optional shadow, clean labels, and circle markers at liquidity grabs. **Automatically fades fill during sideways markets using KDJ(9,3) detection for cleaner charts.**
- Performance Optimized: Huge performance improvement. Limits lines/labels to prevent lag; uses safe array management and processes only recent bars.

Alerts:
- Trend Up: Trend has changed to Up
- Trend Down: Trend has changed to Down
- Trend Changed: Trend has changed to {{strategy.order.action}} (auto shows "up" or "down")
- Trend Direction Changed: Trend has changed direction

Ideal for trend-following, liquidity hunting, and volume-confirmed reversals. Clean, efficient, and highly visual.
