# Automation & Web Scraping Toolkit 🚀

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-Automation-green?style=flat-square&logo=selenium&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-orange?style=flat-square&logo=pandas&logoColor=white)

A robust, production-ready collection of Python scripts engineered for secure communication, advanced browser automation, dynamic web scraping, and reliable background task scheduling.

---

## 📋 Script Summary Matrix

| File Name | Primary Category | Key Dependencies | Output / Action |
| :--- | :--- | :--- | :--- |
| `file1_email.py` | Communication | `smtplib`, `ssl` | Secure SMTP email dispatch via Gmail App Passwords |
| `file2_download.py` | Browser Automation | `selenium` | Automated file download verification from a Heroku staging environment |
| `file3_register.py` | Form Automation | `selenium` | Automated form navigation and submission on DemoQA |
| `file4_duckduckgo.py` | Web Scraping | `selenium`, `pandas` | Scrapes DuckDuckGo search queries and exports data to `Python.csv` |
| `file5_youtube_list.py` | Web Scraping | `selenium`, `pandas` | Extracts top 10 YouTube video titles and links into `YouTube.csv` |
| `file6_youtube_play.py` | Browser Automation | `selenium`, `urllib` | Custom User-Agent injection, search encoding, and window minimization |
| `file7_scheduler.py` | Task Orchestration | `schedule` | Lightweight background task runner executing daily at 21:05 |

---

## 🔍 Detailed Script Breakdown

<details>
<summary><b>1. file1_email.py — Secure SMTP Email Dispatcher</b></summary>

* **Purpose:** Establishes an encrypted connection to Google's SMTP server to dispatch automated email notifications programmatically.
* **Technical Highlight:** Utilizes secure socket layering (`SMTP_SSL`) combined with Google App Passwords to securely authenticate and bypass multi-factor authentication constraints without exposing plaintext credentials.
</details>

<details>
<summary><b>2. file2_download.py — Automated File Downloader</b></summary>

* **Purpose:** Automates browser interactions to locate, trigger, and verify file downloads from a Heroku testing staging site.
* **Technical Highlight:** Configures custom Chrome WebDriver download preferences (`prefs`) to suppress native save-as dialogs and direct downloads straight to a localized target directory.
</details>

<details>
<summary><b>3. file3_register.py — Interactive Form Submission Automation</b></summary>

* **Purpose:** Programmatically navigates, fills out, and submits complex account registration forms on the DemoQA testing platform.
* **Technical Highlight:** Employs precise `By` locators, explicit wait conditions (`WebDriverWait`), and JavaScript execution workarounds to interact seamlessly with obscured or dynamic DOM elements.
</details>

<details>
<summary><b>4. file4_duckduckgo.py — Search Engine Scraper & Exporter</b></summary>

* **Purpose:** Accepts custom user input queries, extracts result titles and corresponding URLs from DuckDuckGo, and structures the data into a tabular format.
* **Technical Highlight:** Integrates Selenium DOM scraping outputs directly into Pandas DataFrames to clean, format, and export records directly to a persistent `Python.csv` file.
</details>

<details>
<summary><b>5. file5_youtube_list.py — YouTube Trend & Search Extractor</b></summary>

* **Purpose:** Scrapes the top 10 video titles and metadata links for any given search query directly from YouTube's dynamic interface.
* **Technical Highlight:** Handles asynchronous DOM loading and infinite scroll states using robust explicit wait conditions before serializing the payload via Pandas into `YouTube.csv`.
</details>

<details>
<summary><b>6. file6_youtube_play.py — Stealth Browser Automation & Navigation</b></summary>

* **Purpose:** Encodes query strings, injects stealth browser configurations, navigates to target platforms, locates video elements, and manages window states.
* **Technical Highlight:** Uses `urllib.parse` for URL encoding, injects custom Mozilla User-Agent strings into `ChromeOptions` to circumvent automated bot detection, and programmatically minimizes the active browser window post-interaction.
</details>

<details>
<summary><b>7. file7_scheduler.py — Lightweight Task Orchestration Engine</b></summary>

* **Purpose:** Orchestrates recurring script execution and background job management at precise, predetermined daily intervals.
* **Technical Highlight:** Implements the Python `schedule` library inside a persistent, low-overhead `while True` loop with periodic tick intervals to trigger target operations reliably every day at 21:05.
</details>

---

## 🛠️ Installation & Quickstart

Clone the repository and install the required dependencies using pip:

```bash
git clone [https://github.com/username/automation-toolkit.git](https://github.com/username/automation-toolkit.git)
cd automation-toolkit
pip install selenium pandas schedule
```

<div align="center">
<hr>
<p><em>Authorized by Rayaan Tasnim</em></p>
</div>
