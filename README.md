# Brute-Forcing-Website
This project is designed to Brute Force the Website and verify the details. It uses selenium for web automation, BeautifulSoup for parsing HTML, and Openpyxl for handling the excel files.

This project automates the process of verifying user details on the website. It utilizes Python libraries such as Selenium for web automation, BeautifulSoup for HTML parsing, and Openpyxl for handling Excel files.

## Prerequisites
Python 3.x
Selenium
BeautifulSoup
Openpyxl
Google Chrome and ChromeDriver

## Usage
1. Prepare the Excel file (passwords.xlsx):
  The Excel file should contain the necessary data structure.
  
2. Prepare the trial_passwords.txt file:
  This file should contain the trial passwords, one per line.

3. Run the script

4. Enter the target username when prompted

## Working

1.Initialize the WebDriver:
  The script initializes a Selenium WebDriver with Chrome options.

2. Process Data:
  The script reads the USN and trial passwords, then submits these details to the website.

3. Verify and Save Results:
  If the details are correct, the script logs the correct password into the correct_password.txt file and updates the Excel sheet (passwords.xlsx).

4.Parallel Processing:
  The script uses multiprocessing to speed up the verification process by handling multiple trial passwords concurrently.

## Notes
Ensure Chrome and ChromeDriver versions are compatible.
Modify the WebDriver initialization (initialize_webdriver) if necessary.
The script currently uses a placeholder path for Chrome binary; update it as per your local installation.

## Security Notice
  Due to security reasons and the potential for misuse on websites lacking proper security measures (e.g., no CAPTCHA or login rate limiting), the full source code for this project is not provided. Automated scripts like this can overwhelm such sites, leading to performance issues or even downtime.

## License
  This project is licensed under the MIT License - see the LICENSE file for details.
