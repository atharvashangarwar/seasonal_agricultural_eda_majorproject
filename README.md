# Seasonal Agriculture Performance Analysis

This is my major project for VOIS AICTE Batch 1 (2026-2027). The task was to analyze a farming dataset and figure out how agricultural performance changes across seasons — Kharif, Rabi and Zaid.

## About the dataset

`seasonal_agriculture_performance_dataset.csv` — 4,000 farm records from 8 Indian states, covering 8 different crops and 4 irrigation methods. Each row has stuff like rainfall, temperature, soil condition, fertilizer/pesticide use, yield, and profit for one farm.

## What I did

Everything is in `Seasonal_Agriculture_Performance_Analysis.ipynb`. Roughly the flow:

- Explored the data first (shape, column types, basic stats)
- Cleaned it up — filled a few missing values (rainfall, soil moisture, yield) using the median for that season instead of just dropping rows
- Checked for duplicates and outliers (found out the "outlier" yield values were just Sugarcane, not bad data)
- Compared yield, profit, and disease/pest risk across the three seasons
- Looked at resource usage (water, fertilizer, pesticide) by season
- Did a correlation check to see what actually drives yield and profit
- Compared crops across seasons and different irrigation methods
- Wrote up findings + a few recommendations at the end

## Main findings (short version)

- Zaid season is the weakest — least rainfall, and about 64% of farms in that season actually lose money
- Kharif has the highest disease/pest risk, probably tied to more rain + humidity
- Drip irrigation gives noticeably better profit than Flood/Rainfed/Sprinkler
- No single factor (soil, weather, etc) explains yield on its own — it's more about crop + season + irrigation together

More detail + all the charts are in the notebook itself.

## How to run it

1. Clone/download this repo
2. Open `Seasonal_Agriculture_Performance_Analysis.ipynb` in Jupyter or Colab
3. Make sure the CSV is in the same folder
4. Run all cells

## Tools used

Python, Pandas, Matplotlib, Seaborn, Google Colab
