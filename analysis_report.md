# Mirza Panel Bot Analysis Report

## 1. Project Architecture
The Mirza Panel bot is a Telegram bot built using **PHP 8.2** and **MySQL**. It uses the **Webhook** method to receive updates from the Telegram API.
The project is hosted on an **Ubuntu 22** server with **Apache2** as the web server, which is fully provisioned and configured via the provided `install.sh` script.

Key Files:
- `index.php`: The main entry point for the bot, handling incoming webhooks and user interactions.
- `admin.php`: Handles all admin-specific commands and functionalities.
- `function.php`: Contains core helper functions for database operations, string manipulation, and API requests.
- `botapi.php`: Handles direct interactions with the Telegram API (e.g., `sendmessage`, `telegram()`).
- `keyboard.php`: Manages the generation of inline and reply keyboards.
- `panels.php`: Contains the `ManagePanel` class, which interfaces with various VPN backends.
- `config.php`: Holds database credentials, bot token, and admin IDs (generated during installation).

## 2. VPN Backend Integrations
The bot supports provisioning and managing VPN configurations across multiple backends:
- **Marzban**
- **X-UI** (including Alireza and Sanaei forks)
- **Hiddify**
- **IBSng**
- **WGDashboard** (WireGuard)
- **MikroTik**

## 3. Payment Gateways
The bot supports a wide variety of payment methods for users to add balance to their wallets or directly purchase services:
- **Crypto / International:** NowPayments, Plisio, Telegram Stars
- **Iranian Gateways:** Zarinpal, Aqayepardakht, Iranpay (multiple currencies), Tronado
- **Manual Payment:** Card-to-Card offline payments with receipt upload and admin verification.

## 4. Bot Logic & Conversation Flow
The bot utilizes a state-machine approach to handle multi-step conversations. This is managed using the `step` column in the `user` table (along with temporary storage in `Processing_value`, `Processing_value_one`, `Processing_value_tow`, etc.).

Common flows include:
- **Purchasing/Extending Service:** Selecting a location -> Choosing a plan -> Applying discount -> Payment -> Provisioning on the target panel.
- **Wallet Top-up:** Entering amount -> Choosing gateway -> Redirecting to payment link / Sending card details -> Confirming payment.
- **Support & Ticketing:** Forwarding user messages to admins, and allowing admins to reply directly to the user's thread.

## 5. Database Schema (Inferred)
The application relies heavily on a relational MySQL database. Key tables include:
- `user`: Stores Telegram IDs, usernames, balances, current conversation `step`, `agent` type, and join metadata.
- `invoice`: Records all purchased services, their target panel (`Service_location`), product names, and current `Status` (e.g., `active`, `end_of_time`).
- `Payment_report`: Tracks pending and completed transactions (`id_order`, `price`, `payment_Status`, `Payment_Method`).
- `product`: Defines the plans available for purchase, constrained by volume, time, and target location.
- `marzban_panel`: Stores the connection details and credentials for the various VPN servers connected to the bot.
- `setting` / `shopSetting` / `PaySetting`: Key-value or JSON configurations managing the bot's behavior, pricing logic, and active modules.
- `Discount` / `DiscountSell`: Manages discount codes and their usage limits.
- `affiliates` / `Requestagent`: Manages the referral system and requests to become an agent (reseller).

## 6. Pre-commit & Testing
The project currently relies on basic PHP syntax checking (`php -l`) for validation. There is no automated unit testing framework (e.g., PHPUnit) configured in the repository.

---
Analysis complete. Ready for further instructions on required changes.
