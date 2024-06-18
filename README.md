# Overview
This script automates the process of logging into LinkedIn, navigating to the user's connected companies, liking posts from these companies, and scraping company information. The script saves this information to an Excel file and keeps track of visited companies to avoid duplicates in future sessions.


# Major Features
## 1. Automated Login.
   * Logs into LinkedIn using saved cookies if available or user credentials.
   * Handles 2FA if required.
## 2. Company Navigation.
   * Navigates to the user's connected companies page on LinkedIn.
## 3. Post Interaction
   * Likes up to 50 posts from each company to increase engagement.
     
## 4. Company Info Scraping:

   * Scrapes company details including name, website, overview, size, and headquarters.Saves the information in an Excel file.

## 5. Visited Companies Tracking:

   * Keeps track of visited companies to avoid duplicate interactions.
     Saves this list for future sessions.

## 6. Error Handling:

   * Handles common exceptions such as timeouts, stale elements, and no such 
     elements.Includes mechanisms to retry actions when needed.

## 7. Periodic Breaks:

   * Pauses the script for 10 minutes after running for an hour to mimic 
     human behavior and avoid being flagged as a bot.

# Installation Steps

1.  install Python: Ensure Python 3.x is installed on your system. You can download it from [python.org](https://www.python.org/).
2.  Clone the Repository.
    ```
    git clone <https://github.com/rajatthakurk/linkedin_post_like_automation.git>
    cd <your-repo-directory>
    ```
3.  Create and Activate Virtual Environment.
    ```
    python -m venv myenv
    source myenv/bin/activate  # On Windows, use `.\myenv\Scripts\activate`
    ```
4.  Install Dependencies.
    ```
    pip install -r requirements.txt
    ```
5. Download ChromeDriver.
   * ChromeDriver is persent in this repo follow below steps for updating ChromeDriver if needed.
   * Download ChromeDriver from [ChromeDriver download page](https://developer.chrome.com/docs/chromedriver/downloads) that matches your 
    Chrome browser version.
   * Extract the downloaded file and place it in a known directory (e.g., chromedriver-win64/chromedriver.exe).
6. Run the Script.
   * Prepare Cookies.
     1. If cookies are not available, the script will ask for LinkedIn username 
        and password. This happens only once, as the script saves cookies for 
        subsequent sessions.
     2. Ensure 2FA is completed if prompted, and press Enter to proceed.
   * Execute the Script.
      1. Open the terminal or command prompt.
      2. Navigate to the directory where linkedin_automation.py is saved.
      3. Run the script by executing:
         ```
         python linkedin_automation.py
         ```
This script is designed to be robust and user-friendly, automating the mundane tasks of interacting with LinkedIn companies and collecting relevant information efficiently.
