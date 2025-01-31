# Hyrox Rankings Web Scraper 🏋️‍♂️📊

This project is a **web scraper** built with **Selenium** and **BeautifulSoup** to extract **global rankings** from [Hyrox PFT Rankings](https://pft.hyrox.com/ranking/global). The script iterates through multiple pages, extracts relevant data, and saves it into a **CSV file**.

## Features 🚀
- **Extracts rankings, names, times, locations, age groups, and medals** from the Hyrox PFT rankings.
- **Handles pagination** automatically to scrape data from multiple pages.
- **Saves data as a CSV file** for further analysis.
- **Headless browsing** for faster and smoother execution.

## Installation 🛠️

1. Clone the repository:
   ```bash
   git clone https://github.com/nishantshah2112/hyrox-rankings-scraper.git
   cd hyrox-rankings-scraper
   ```

2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the script:
   ```bash
   python scrape_hyrox_rankings.py
   ```

## Dependencies 📦
This script requires the following Python libraries:
- `selenium`
- `webdriver-manager`
- `beautifulsoup4`
- `pandas`

Install them using:
```bash
pip install selenium webdriver-manager beautifulsoup4 pandas
```

## Output 📄
The extracted data is saved in **CSV format**:
```
hyrox_rankings.csv
```

### CSV Structure:
| Rank | Name | Time | Location | Age Group | Medal |
|------|------|------|----------|-----------|-------|
| 1    | John Doe | 00:42:15 | New York, USA | 30-34 | Gold |
| 2    | Jane Smith | 00:45:30 | London, UK | 25-29 | Silver |
| ...  | ...  | ...  | ...  | ...  | ... |

## How It Works 🔍
1. **Opens the Hyrox rankings page** using Selenium.
2. **Extracts data** using BeautifulSoup.
3. **Navigates through pages** by clicking the "Next page" button.
4. **Saves all extracted data** into `hyrox_rankings.csv`.

## Notes 📝
- This script **runs in headless mode** by default. To disable headless mode for debugging, remove:
  ```python
  chrome_options.add_argument("--headless")
  ```
- Ensure you have **Google Chrome installed** with the latest **ChromeDriver**.

## License 📜
This project is licensed under the **MIT License**.

## Author 👨‍💻
Developed by [Nishant Shah](https://github.com/nishantshah2112).
