Here's the updated README without the "Need Help? Contact & Support" section:

---

# 🚀 **Ultimate Bot Setup Guide**

Welcome! This guide will walk you through the **installation and configuration** process to get your bot up and running. It’s crafted to ensure even first-time users can set things up without breaking a sweat.

---

## **Table of Contents**

1. [Prerequisites](#prerequisites)
2. [Step-by-Step Installation](#step-by-step-installation)
3. [Configuration Files](#configuration-files)
   - [`configs.json`](#1-configsjson)
   - [`datas.txt`](#2-datastxt)
   - [`wallets.txt`](#3-walletstxt)
   - [`proxies.txt`](#4-proxiestxt)
4. [Running the Bot](#running-the-bot)

---

## **1. Prerequisites**

Before you dive in, make sure you have the following installed:

- **Node.js** (Version: `22.11.0`)
- **npm** (Version: `10.9.0`)

👉 Download Node.js and npm: [Official Download Link](https://nodejs.org)

---

## **2. Step-by-Step Installation**

1. **Download and Extract:**
   - Get the bot package and unzip it into a folder on your computer.

2. **Install Dependencies:**
   Open a terminal, navigate to the folder, and run the following command:

   ```bash
   npm install user-agents axios colors p-limit https-proxy-agent socks-proxy-agent crypto-js ws uuid xlsx readline-sync
   ```

3. **Configure Settings:**
   - Prepare the necessary configuration files as detailed below.

---

## **3. Configuration Files**

### **1. `configs.json`** – *Control the Bot’s Behavior*

Here’s a sample configuration you can tweak:

```json
{
  "timeZone": "en-US",
  "rotateProxy": false,
  "skipInvalidProxy": false,
  "proxyRotationInterval": 2,
  "delayEachAccount": [5, 8],
  "timeToRestartAllAccounts": 300,
  "howManyAccountsRunInOneTime": 100,
  "doTasks": true,
  "playGames": true,
  "referralCode": "687WN6G3LOZR",
  "amountOfUpgrades": 10
}
```

- **Key Fields:**
  - `timeZone`: Set your time zone (e.g., `"en-US"`).
  - `rotateProxy`: Enable or disable proxy rotation.
  - `skipInvalidProxy`: Skip invalid proxies automatically.
  - `delayEachAccount`: Range (in seconds) of delays between accounts.
  - `howManyAccountsRunInOneTime`: Number of simultaneous accounts.
  - `referralCode`: Enter a referral code here to support developers (or your own).
  - `amountOfUpgrades`: Number of account upgrades to execute.

---

### **2. `datas.txt`** – 🗂️ *User Information*

Fill this file with user data in the format:

```txt
query_id.../user...
query_id.../user...
query_id.../user...
```

👉 Download an example file [here](https://t.me/KeoAirDropFreeNe/257/6879).

---

### **3. `wallets.txt`** – 💼 *EVM Wallet Addresses*

Add your wallet addresses (one per line) like this:

```txt
0xYourAddressHere
0xAnotherAddressHere
```

---

### **4. `proxies.txt`** – 🌐 *Proxy Settings*

If using proxies, add them in the following formats (one per line):

```txt
http://user:password@host:port
https://user:password@host:port
socks4://user:password@host:port
socks5://user:password@host:port
```

Leave the file blank if not using proxies.

---

## **4. Running the Bot**

Now the fun part! Follow these steps:

1. Open a terminal and navigate to the bot directory:

   ```bash
   cd /path/to/bot-folder
   ```

2. Start the bot with this command:

   ```bash
   node coffin
   ```

---

Enjoy exploring the bot, and happy automating! 🚀
