# Jersey Weather Scraper

Automated daily collection and archival of Jersey (Channel Islands) weather data from the official Jersey Met API.

## What it does

This repository automatically scrapes weather data from `https://prodgojweatherstorage.blob.core.windows.net/data/jerseyForecast.json` every day at 10:30 AM UTC and stores it in multiple formats:

- **Current data**: Today's processed weather conditions (`data/current/jersey-weather-today.json`)
- **Raw archive**: Daily snapshots of complete API responses (`data/archive/jersey-weather-raw-YYYY-MM-DD.json`)
- **Analysis dataset**: Consolidated historical data for trends and analysis (`data/jersey-weather-analysis.json`)

## Data collected

- Current temperature and conditions
- Today's weather summary and detailed descriptions
- Temperature ranges (min/max in °C and °F)
- Wind speed and direction
- Rain probabilities throughout the day
- UV index and sunrise/sunset times

## Automation

Runs via GitHub Actions daily with automatic git commits. No manual intervention required.

## Built with

- GitHub Actions for automation
- Node.js for data processing
- Jersey Met Office API
- Designed with assistance from Claude Sonnet 4

## License

MIT License - see LICENSE file for details.