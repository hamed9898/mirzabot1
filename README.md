# 🤖 Bot Mirza Panel

A Powerful Bot for Selling VPN Services with Auto Configuration Build.

<p align="center">
    <a href="https://t.me/mirzapanel" target="_blank">
        <img src="https://img.shields.io/badge/Telegram-Group-blue?style=flat-square&logo=telegram" alt="Telegram Group"/>
    </a>
    <a href="https://github.com/mahdiMGF2/mirzabot" target="_blank">
        <img src="https://img.shields.io/github/stars/mahdiMGF2/mirzabot?style=social" alt="GitHub Stars"/>
    </a>
    <a href="https://img.shields.io/github/forks/mahdiMGF2/mirzabot?style=flat-square" target="_blank">
        <img src="https://img.shields.io/github/forks/mahdiMGF2/botmirzapanel?style=flat-square" alt="GitHub Forks"/>
    </a>
    <a href="https://github.com/mahdiMGF2/botmirzapanel/issues" target="_blank">
        <img src="https://img.shields.io/github/issues/mahdiMGF2/mirzabot?style=flat-square" alt="GitHub Issues"/>
    </a>
</p>

---

## 📚 Table of Contents

- [✨ Overview](#-overview)
- [🧩 Supported Panels](#-supported-panels)
- [⚙️ Features](#️-features)
- [💻 Technologies Used](#-technologies-used)
- [🚀 Installation](#-installation)
  - [Prerequisites](#prerequisites)
  - [Installing the Bot](#-installing-the-bot-stable-version)
  - [Updating the Bot](#-updating-bot)
  - [Removing the Bot](#-removing)
- [🌐 Web Admin Panel](#-web-admin-panel)
- [💵 Financial Support](#-financial-support)
- [🌍 Persian / فارسی](#-persian--فارسی)

---

## ✨ Overview

**Mirza Bot** is a feature-rich Telegram bot designed for selling VPN services. It streamlines your VPN business by offering automated subscription sales, seamless configuration generation, payment processing, and comprehensive user and panel management.

Mirza Panel is available in two versions:
1. **Free Version** 🆓: Essential tools and features to start and run your VPN sales.
2. **Subscription Version** 💎: Advanced business features, robust customization, detailed analytics, and enhanced control.

Whether you are offering simple trial accounts or managing a large-scale VPN infrastructure, Mirza Panel covers all your needs.

---

## 🧩 Supported Panels

Mirza Panel natively integrates with the most popular VPN management panels:
- **Marzban**
- **X-UI** (including Alireza & Sanaei forks)
- **Hiddify**
- **IBSng**
- **WGDashboard** (WireGuard)
- **MikroTik**

---

## ⚙️ Features

### 🔹 **Free Version Features**

- ✅ **Automated Service Delivery**: Auto-configuration creation after VPN purchase.
- ✅ **User Management**: View purchased services, support section, and trial accounts.
- ✅ **Authentication**: Phone number verification for enhanced security.
- ✅ **Flexible Payments**:
  - Manual Card-to-Card
  - **NowPayments** Gateway (Crypto)
  - **aqayepardakht** Gateway (IR Rial)
- ✅ **Multi-Protocol**: Full compatibility with modern proxy protocols (V2Ray, WireGuard, etc.).
- ✅ **Marketing Tools**: Mandatory channel membership to use the bot.
- ✅ **Reports & Analytics**: Detailed reports for purchases and trial usages.
- ✅ **Admin Controls**:
  - Balance management and multiple admins support.
  - Renewals, volume top-ups, config retrieval, and link updates.
  - Product, gateway, and panel management.
  - Fully customizable text, FAQ, and tutorials from within the bot.
- ✅ **Smart Configs**: Protocol-specific configuration settings and admin-defined username generation patterns.

### 🔹 **Subscription Version Features**

Includes all Free features plus powerful enhancements for serious businesses.

📌 **Subscription Purchase Guide**: [View Guide](https://t.me/mirzaperimium/4)

---

## 💻 Technologies Used

- **Language:** PHP 8.x
- **Database:** MySQL / MariaDB (using PDO & mysqli)
- **API:** Telegram Bot API
- **Web Interface:** HTML, CSS, JavaScript (for the Web Admin Panel)
- **Integration:** Webhooks and cron jobs for seamless real-time processing

---

## 🚀 Installation

### Prerequisites

Ensure you have the following before installation:
- 🖥️ **Ubuntu Server 22.04** (Recommended)
- 🌐 **A Domain Name** (Pointed to your server IP)

### 🔧 Installing the Bot (Stable Version)

Run the following command in your server terminal:

```bash
curl -o install.sh -L https://raw.githubusercontent.com/mahdiMGF2/mirzabot/main/install.sh && bash install.sh
```

When prompted, **select option 1** to complete the installation. Follow the on-screen prompts to configure your domain and Telegram bot token.

### 🔄 Updating Bot

To update your bot to the latest version, run the installer again:

```bash
curl -o install.sh -L https://raw.githubusercontent.com/mahdiMGF2/botmirzapanel/main/install.sh && bash install.sh
```
When prompted, **select the update option**.

### ❌ Removing

If you wish to completely uninstall the bot from your server:

```bash
curl -o install.sh -L https://raw.githubusercontent.com/mahdiMGF2/botmirzapanel/main/install.sh && bash install.sh
```
When prompted, **select option 3** to remove the bot.

---

## 🌐 Web Admin Panel

Mirza Panel includes a sleek web-based admin dashboard for easier management.
Once installed, you can access your panel by navigating to your domain. The default path is usually under the `panel/` directory.

- Features: Manage users, adjust settings, track payments, and manage products directly from your browser.
- Path: `https://yourdomain.com/panel`

---

## 💵 Financial Support

If you find **Mirza Panel** helpful and want to support its active development, consider making a financial contribution via cryptocurrency:

<a href="https://nowpayments.io/donation/permiumbotmirza">👉 Support the Project on NowPayments</a>

Your support ensures continuous updates and improvements. Thank you! 🙌

---

## 🌍 Persian / فارسی

این ربات به صورت پیش‌فرض برای کاربران ایرانی طراحی شده و تمامی متون آن فارسی است (قابل تغییر در ربات و پنل). برای راهنمایی بیشتر و ارتباط با جامعه کاربری، به گروه تلگرامی ما بپیوندید:
[گروه تلگرام Mirza Panel](https://t.me/mirzapanel)

---

### Contributors

![Contributors](https://contrib.rocks/image?repo=mahdiMGF2/mirzabot)
