# Dream11 Automation

This project automates the generation of Dream11 teams by fetching live data, analyzing past performance, and generating balanced teams.

## Features

- Fetches live data from Dream11 API.
- Analyzes past player performance.
- Generates multiple teams based on live and past data.

## Requirements

- Python 3.8+
- `requests`, `pandas`, and `python-dotenv` libraries.

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/dream11-automation.git
   cd dream11-automation
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Create `.env` file with your API token:
   ```plaintext
   DREAM11_ACCESS_TOKEN=your_api_access_token_here
   ```

4. Add past performance data in `data/megha_team_stats.csv`.

5. Run the script:
   ```bash
   python dream11_automation.py
   ```

## File Structure

```
dream11-automation/
│
├── data/
│   └── megha_team_stats.csv      # Past performance data (input file)
│
├── .env                         # Environment variables (API token, etc.)
├── requirements.txt             # Python dependencies
├── dream11_automation.py        # Main automation script
├── README.md                    # Documentation
```

## Notes

- Ensure valid API token is added in `.env` file.
- Past data file should have a `performance_score` column.
- Modify the `generate_teams` function for custom team logic.
