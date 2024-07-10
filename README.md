# Formula-1-Project

# Formula 1 Standings Scraper

This Python script scrapes Formula 1 driver and team standings data from the official Formula 1 website for the years 1950 to 2023 and saves the data as individual CSV files.

## Features

- Scrapes driver and team standings data from formula1.com
- Covers all Formula 1 seasons from 1950 to 2023
- Saves data for each year as separate CSV files for drivers and teams
- Includes position, full name, nationality, car, and points for each driver
- Includes position, team name, and points for each team

## Requirements

- Python 3.x
- Required libraries:
  - requests
  - BeautifulSoup4
  - pandas

## Installation

1. Clone this repository or download the script.
2. Install the required libraries:

```
pip install requests beautifulsoup4 pandas
```

## Usage

1. Run the script:

```
python f1_scraper.py
```

2. The script will create two directories: `f1_driver_standings` and `f1_team_standings` (if they don't exist) and save individual CSV files for each year's standings in these directories.

3. Each CSV file will be named in the format `f1_driver_standings_YYYY.csv` or `f1_team_standings_YYYY.csv`, where YYYY is the year.

## Output

### Driver Standings CSV files contain:

- Position
- Full Name
- Nationality
- Car
- Points

### Team Standings CSV files contain:

- Position
- Team
- Points

## Notes

- The script includes a 1-second delay between requests to avoid overwhelming the server.
- If no data is found for a particular year, the script will print a message indicating this.
- Team standings data may not be available for all years, especially in the earlier seasons of Formula 1.
- This script is for educational purposes only. Please respect the terms of service of formula1.com when using this script.

## License

This project is open source and available under the [MIT License](LICENSE).
