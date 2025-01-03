
# Hydrion-S3LFB0T

## Quick Setup

### For Windows Users 💻
1. Install **Git** from https://git-scm.com/download/win and **Node.js** from https://nodejs.org/en/download/.
2. Open **Command Prompt** or **PowerShell** and run the following commands:

```bash
git clone https://github.com/Hydrion-Tools/Hydrion-S3LFB0T.git
cd Hydrion-S3LFB0T
```
3. Then add your token and prefix in **config.json**.

4. Use the command below to **Install** all dependency

```bash
npm install
```

5. Now **Start** the bot using the command below

This will set up your bot with all required dependencies.

---

### For Termux (Android Mobile Users) 📱
1. Install **Termux** from the Google Play Store.
2. Open **Termux** and run the following commands:

```bash
pkg install git -y
git clone https://github.com/Hydrion-Tools/Hydrion-S3LFB0T.git
cd Hydrion-S3LFB0T
bash setup.sh
```

3. To edit the **config.json** Use the command below

```bash
nano config.json
```

This will install all the required dependencies and set up the bot.

---

## Running the Bot with PM2 🚀

### What is PM2?
**PM2** is a process manager for Node.js applications that will keep your bot running even if your session ends. It also makes it easier to start, stop, and monitor the bot.

### How to Start the Bot
Once the setup is complete and the `setup.sh` script has run, your bot should automatically start using **PM2**. However, if you need to start it manually, run:

```bash
pm2 start bot.js --name "hydrion-selfbot"
```

### Saving the PM2 Process List
To ensure that your bot starts automatically when the server restarts, run:

```bash
pm2 save
```

### Stopping the Bot
To stop the bot running with PM2, you can use:

```bash
pm2 stop "hydrion-selfbot"
```

### Restarting the Bot
If you need to restart the bot, run:

```bash
pm2 restart "hydrion-selfbot"
```

---

## Configuration ⚙️

After the setup, you will be prompted to enter your **Discord Token**. This is required to run the bot. The token will be saved in a `config.json` file, which the bot will read during execution.

---

## Troubleshooting ⚠️

- If you encounter any issues, ensure that **Node.js** and **Git** are correctly installed.
- You can check the status of the bot using PM2 by running:

```bash
pm2 status
```

If you need to view the logs for debugging:

```bash
pm2 logs "hydrion-selfbot"
```

---

### Contact 📩

If you have any questions or need support, feel free to contact us via the [Hydrion Support Discord](https://discord.gg/6Tufbvnebj).

---

**Selfbot crafted by** `@hydradevx` 🎨