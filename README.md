# Multi-Currency Revenue Reporter

## What it does
This tool converts monthly hotel booking revenue from INR into a selected foreign currency (USD, EUR, or GBP) using historical exchange rates from the Frankfurter API.

## How to run
1. Open the notebook `fx_reporter.ipynb`.
2. Upload the dataset `hotel_bookings (1).csv`.
3. Run all notebook cells.
4. Enter the desired currency (USD, EUR, or GBP).

## Design Decision
Historical monthly exchange rates were used instead of current exchange rates so that revenue trends reflect the actual exchange rate applicable during each period.

## Limitation
The tool uses one exchange rate per month and depends on Frankfurter API availability. Missing API responses may result in unavailable converted values for some months.
