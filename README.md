# Twitter-Scrapper

```markdown
# Twitter Scraper

This is a Python-based Twitter profile scraper using **Selenium and Firefox WebDriver**.  
The script extracts **Twitter Bio, Followers Count, Following Count, Location, and Website** from public profiles.  

## Features
- Scrapes **Twitter profile details** (Bio, Followers, Following, Location, Website).  
- Uses **Selenium WebDriver** for automation.  
- Reads Twitter usernames from a **CSV file**.  
- Saves the scraped data to a **CSV output file**.  
- Works in **Google Colab & Local Machine** (Windows/Linux).  

---

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/kavyakapoor200/Twitter-Scrapper.git
cd Twitter-Scrapper
```

### 2. Install Required Packages
```bash
pip install selenium gdown pandas
```

### 3. Download & Install Firefox WebDriver
- **Linux Users (Google Colab)**: No additional setup is required.  
- **Windows Users**: [Download GeckoDriver](https://github.com/mozilla/geckodriver/releases) and add it to PATH.  

---

## Usage

### 1. Prepare the Input CSV
Ensure you have a **CSV file** (`twitter_profiles.csv`) containing Twitter profile URLs.  

### 2. Run the Scraper
```bash
python Twitter_Scrapper.ipynb
```
OR in Jupyter Notebook:
```python
!python Twitter_Scrapper.ipynb
```

### 3. View the Output
- The scraped data will be saved in **`scraped_twitter_data.csv`**.  
- Open it in **Excel** or **Pandas** for analysis.  

---

## Troubleshooting

### Missing Data ("Not Available")
- Twitter has strict anti-bot measures, which may cause some fields to be unavailable.  
- Try **running in non-headless mode** by removing the `--headless` option in Selenium.  
- Increase the **wait time (`time.sleep(7-12)`)** to ensure elements load properly.  
- If too many requests are made in a short time, **Twitter may temporarily block the IP**.  

### Selenium Not Working
- Ensure that **Firefox & GeckoDriver** are installed.  
- Try updating Selenium with:
```bash
pip install --upgrade selenium
```

---

## Contributing
Contributions are welcome. If you have any improvements, feel free to **fork the repository** and submit a **pull request**.  

---

## License
This project is licensed under the **MIT License**.  

---

### Author
Developed by [kavyakapoor200](https://github.com/kavyakapoor200).
```
