<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
</head>
<body>

<h1>WhatsApp Auto-Wisher</h1>
<p>This Python script automates the process of sending birthday wishes via WhatsApp. It reads an Excel file with contact details, checks if today is anyone's birthday, and sends a personalized message to the birthday person through WhatsApp. The script is scheduled to run daily using the Windows Task Scheduler.</p>

<h2>Features</h2>
<ul>
    <li>Reads contact information, birthday, and personalized message from an Excel sheet.</li>
    <li>Automatically sends birthday wishes via WhatsApp using pywhatkit.</li>
    <li>Set to run daily through Windows Task Scheduler.</li>
</ul>

<h2>Technologies Used</h2>
<ul>
    <li><strong>Python</strong>: Core programming language.</li>
    <li><strong>Libraries</strong>:
        <ul>
            <li><code>pandas</code>: For reading and managing Excel files.</li>
            <li><code>openpyxl</code>: For Excel file handling.</li>
            <li><code>pyautogui</code>: For GUI automation.</li>
            <li><code>pywhatkit</code>: For sending messages via WhatsApp.</li>
            <li><code>datetime</code>: For handling date comparisons.</li>
            <li><code>xlrd</code>: For reading older Excel formats (.xls).</li>
            <li><code>time</code>: For handling delays.</li>
        </ul>
    </li>
</ul>

<h2>Installation</h2>
<ol>
    <li>Clone the repository:
        <pre><code>git clone https://github.com/yourusername/whatsapp-auto-wisher.git</code></pre>
    </li>
    <li>Install the required dependencies:
        <pre><code>pip install pandas openpyxl pywhatkit pyautogui xlrd</code></pre>
    </li>
    <li>Add your Excel file (e.g., <code>birthdays.xlsx</code>) to the project directory. The Excel sheet should contain columns for:
        <ul>
            <li>WhatsApp Number</li>
            <li>Birthday (in <code>YYYY-MM-DD</code> format)</li>
            <li>Message</li>
        </ul>
    </li>
</ol>

<h2>Usage</h2>
<ol>
    <li>Set up the project to run automatically using Windows Task Scheduler:
        <ul>
            <li>Open Task Scheduler and create a new task.</li>
            <li>Set the task to trigger daily.</li>
            <li>In the actions tab, set the action to run the Python script on your local machine.</li>
        </ul>
    </li>
    <li>Ensure that WhatsApp Web is connected on your browser and that the browser remains open.</li>
    <li>The script will check for any matching birthdays in the Excel sheet. If a match is found, it will send the personalized birthday message to the respective WhatsApp contact.</li>
</ol>




<h2>Contributions</h2>
<p>This project was created by <strong>Suryanath Tripathy</strong>. Feel free to fork this repository and make your own improvements. Pull requests are welcome!</p>

<h2>License</h2>
<p>This project is licensed under the MIT License. See the LICENSE file for details.</p>

</body>
</html>
