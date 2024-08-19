

WhatsApp Auto-Wisher
This Python script automates the process of sending birthday wishes via WhatsApp. It reads an Excel file with contact details, checks if today is anyone's birthday, and sends a personalized message to the birthday person through WhatsApp. The script is scheduled to run daily using the Windows Task Scheduler.

Features
Reads contact information, birthday, and personalized message from an Excel sheet.
Automatically sends birthday wishes via WhatsApp using pywhatkit.
Set to run daily through Windows Task Scheduler.
Technologies Used
Python: Core programming language.
Libraries:
pandas: For reading and managing Excel files.
openpyxl: For Excel file handling.
pyautogui: For GUI automation.
pywhatkit: For sending messages via WhatsApp.
datetime: For handling date comparisons.
xlrd: For reading older Excel formats (.xls).
time: For handling delays.
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/whatsapp-auto-wisher.git
Install the required dependencies:

bash
Copy code
pip install pandas openpyxl pywhatkit pyautogui xlrd
Add your Excel file (e.g., birthdays.xlsx) to the project directory. The Excel sheet should contain columns for:

WhatsApp Number
Birthday (in YYYY-MM-DD format)
Message
Usage
Set up the project to run automatically using Windows Task Scheduler:

Open Task Scheduler and create a new task.
Set the task to trigger daily.
In the actions tab, set the action to run the Python script on your local machine.
Ensure that WhatsApp Web is connected on your browser and that the browser remains open.

The script will check for any matching birthdays in the Excel sheet. If a match is found, it will send the personalized birthday message to the respective WhatsApp contact.

Example
python
Copy code
import pandas as pd
import xlrd
import openpyxl
import pyautogui
import time
import pywhatkit
import datetime

# Your script code here...
Contributions
This project was created by Suryanath Tripathy. Feel free to fork this repository and make your own improvements. Pull requests are welcome!

License
This project is licensed under the MIT License. See the LICENSE file for details.
