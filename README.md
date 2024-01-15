# FVGs

## Description
The FVGs (Fair Value Gaps) program is a forex trading robot developed by the Forex Robot Easy Team. It is designed to identify and highlight Fair Value Gaps on the trading chart. Fair Value Gaps occur when the price of an asset deviates significantly from its fair value, presenting potential trading opportunities.

## Developer
This program has been developed by the Forex Robot Easy Team, a group of experienced forex traders and developers. Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that demonstrates how the program works.

## Developer's Site
For detailed reviews and trading results of this product, please visit the official developer's website at [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/fvg-forex-software-review-smart-trading-with-fair-value-gaps/).

## Input Parameters
- **timePeriod** (default: PERIOD_M5): Specifies the time period for analyzing the fair value gaps. The default time period is M5 (5-minute chart).
- **longFVGColor** (default: clrGreen): Specifies the color for highlighting long fair value gaps on the trading chart. The default color is Green.
- **shortFVGColor** (default: clrRed): Specifies the color for highlighting short fair value gaps on the trading chart. The default color is Red.
- **middlePointColor** (default: clrYellow): Specifies the color for highlighting the middle point of fair value gaps on the trading chart. The default color is Yellow.

## Global Variables
- **fvgTimestamps**: Array to store the timestamps of fair value gaps.
- **fvgDirections**: Array to store the directions (Long or Short) of fair value gaps.
- **fvgMiddlePoints**: Array to store the middle points of fair value gaps.

## Functions
- **FindFVGs()**: Identifies and highlights fair value gaps on the trading chart.
- **PlotFVG(int index)**: Plots the fair value gaps on the trading chart.
- **BacktestFVGs()**: Performs backtesting analysis using the fair value gap data.

## How It Works
1. The program starts by calling the **FindFVGs()** function, which loops through the bars on the chart and identifies fair value gaps based on the previous and current highs and lows.
2. If a long fair value gap is detected (currentHigh < previousLow), the program stores the timestamp, direction (Long), and middle point of the fair value gap in the respective arrays.
3. If a short fair value gap is detected (currentLow > previousHigh), the program stores the timestamp, direction (Short), and middle point of the fair value gap in the respective arrays.
4. The **PlotFVG(int index)** function is called to plot the fair value gaps on the trading chart using arrows and lines. The color of the arrows and lines is determined by the input parameters.
5. The **BacktestFVGs()** function is called to perform backtesting analysis using the fair value gap data. This allows traders to analyze the performance and profitability of trading based on fair value gaps.

## Usage
To use this program, follow these steps:
1. Set the desired input parameters according to your trading preferences.
2. Run the program.
3. The program will identify and highlight fair value gaps on the trading chart.
4. You can analyze the fair value gaps visually on the chart or perform backtesting analysis using the fair value gap data.

Please note that this program is provided as a sample code and is not the official product. To find the official developer of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/fvg-forex-software-review-smart-trading-with-fair-value-gaps/).
