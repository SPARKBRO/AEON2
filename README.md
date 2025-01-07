![](https://github.com/5hojib/5hojib/raw/main/images/Aeon-MLTB.gif)

---

# Aeon Bot

Aeon is a streamlined and feature-rich bot designed for efficient deployment and enhanced functionality.

---

## Features

- **Minimalistic and Optimized**: Simplified by removing unnecessary code for better performance.
- **Effortless Deployment**: Fully configured for quick and easy deployment to Heroku.
- **Enhanced Capabilities**: Integrates features from multiple sources to provide a versatile bot experience.

---

## Deployment Instructions (Heroku)

Follow these steps to deploy Aeon to Heroku:

### 1. Clone the Repository
- Clone [This](https://github.com/Hrishi2861/Aeon-Modified) Repository On Your Local Machine.
- Give the repository a star to show your support.

### 2. Navigate to Cloned Repository
- Open the Terminal In That Folder.

### 3. Install Heroku CLI (Skip if Already Installed)
- Windows: [x64](https://cli-assets.heroku.com/channels/stable/heroku-x64.exe) [x32](https://cli-assets.heroku.com/channels/stable/heroku-x86.exe) 
- Mac: `$ brew tap heroku/brew && brew install heroku`
- Linux: `$ curl https://cli-assets.heroku.com/install.sh | sh`

### 4. Create A Heroku App.
1. Open the [Heroku DashBoard](https://dashboard.heroku.com) and Login.
2. Create a Heroku App.

### 5. Set Required Config Vars.
1. Go to Heroku App Settings.
2. Click on **Reveal Config Vars**. and fill out the required inputs:
   - **BOT_TOKEN**: Your Telegram bot token.
   - **OWNER_ID**: Your Telegram ID.
   - **DATABASE_URL**: MongoDB connection string.
   - **TELEGRAM_API**: Telegram API ID (from [my.telegram.org](https://my.telegram.org/)).
   - **TELEGRAM_HASH**: Telegram API hash (from [my.telegram.org](https://my.telegram.org/)).

### 6. Deploy Aeon Repository on Heroku App.
1. Set Git Remote to Heroku App: `heroku git:remote {App_Name}`
2. Set Container as Stack: `heroku stack:set container`
3. Push the Repository: `git push heroku deploy:master -f`
5. Run the workflow and wait for it to complete.

### 7. Finalize Setup
- After deployment, configure any remaining variables in your Heroku dashboard.
- Use the `/bsettings` command to upload sensitive files like `token.pickle` if needed.

---

## Contributing

We welcome contributions! Whether it's bug fixes, feature enhancements, or general improvements:
- **Report issues**: Open an issue for bugs or suggestions.
- **Submit pull requests**: Share your contributions with the community.

---

## License

This project is licensed under the MIT License. Refer to the [LICENSE](LICENSE) file for details.

---

## Acknowledgements

- Special thanks to the original developers of the [Mirror-Leech-Telegram-Bot](https://github.com/anasty17/mirror-leech-telegram-bot).
- Gratitude to contributors from various repositories whose features have been integrated into Aeon.