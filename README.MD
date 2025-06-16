# 🤖 Discord Account Generator Bot

<div align="center">

![Python](https://img.shields.io/badge/Python-3.xx-blue.svg)
![Discord.py](https://img.shields.io/badge/discord.py-green.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)
![Status](https://img.shields.io/badge/Status-Active-brightgreen.svg)

*A powerful Discord bot for generating and managing accounts with premium features and advanced security*

[Features](#-features) • [Installation](#-installation) • [Configuration](#-configuration) • [Commands](#-commands) • [Premium](#-premium-system)

</div>

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [🚀 Installation](#-installation)
- [⚙️ Configuration](#️-configuration)
- [🎯 Commands](#-commands)
- [💎 Premium System](#-premium-system)
- [🔒 Security Features](#-security-features)
- [📊 Statistics](#-statistics)
- [🆘 Support & Help](#-support--help)
- [📝 License](#-license)

---

## ✨ Features

### 🎮 **Core Functionality**
- **Account Generation**: Generate accounts for multiple services
- **Premium System**: Advanced features for premium users
- **Cooldown Management**: Smart cooldown system with premium benefits
- **Auto-completion**: Service auto-completion for better UX
- **DM Delivery**: Secure account delivery via direct messages

### 🔐 **Security & Access Control**
- **Whitelist System**: Server and user-based access control
- **Premium Keys**: Secure premium access management
- **Channel Restrictions**: Command usage limited to specific channels
- **Auto-moderation**: Automatic message deletion in generation channels

### 📈 **Management Features**
- **Stock Management**: Real-time account stock tracking
- **Restock Notifications**: Automated restock announcements
- **Statistics Tracking**: Comprehensive usage analytics
- **Service Creation**: Dynamic service management

---

## 🚀 Installation

### Prerequisites
- Python 3.11 or higher
- Discord Bot Token
- Discord Server with appropriate permissions

### Quick Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/gxqk/spec-x-gen-discord-bot.git
   cd discord-account-generator-bot
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure the bot**
   ```bash
   cp config1.json config.json
   # Edit config.json with your settings
   ```

4. **Run the bot**
   ```bash
   python main.py
   ```

---

## ⚙️ Configuration

### 📄 config.json

```json
{
    "token": "YOUR_DISCORD_BOT_TOKEN",
    "status_type": "streaming",
    "normal_cooldown": 450,
    "premium_cooldown": 60,
    "normal_channel_generation": "CHANNEL_ID",
    "premium_channel_generation": "CHANNEL_ID",
    "premium_role": "ROLE_ID",
    "generate_gif": "GIF_URL",
    "restock_gif": "GIF_URL",
    "cooldown_gif": "GIF_URL",
    "whitelist": ["USER_ID_1", "USER_ID_2"],
    "whitelist_guilds": ["GUILD_ID_1", "GUILD_ID_2"],
    "colors": {
        "success": "0x9b59b6",
        "error": "0x71368a",
        "info": "0x8e44ad"
    }
}
```

### 🔧 Configuration Options

| Option | Description | Type |
|--------|-------------|------|
| `token` | Discord bot token | String |
| `status_type` | Bot status type (playing, streaming, etc.) | String |
| `normal_cooldown` | Cooldown for regular users (seconds) | Integer |
| `premium_cooldown` | Cooldown for premium users (seconds) | Integer |
| `whitelist` | Array of whitelisted user IDs | Array |
| `whitelist_guilds` | Array of whitelisted server IDs | Array |

---

## 🎯 Commands

### 🎮 **Generation Commands**

#### `/generate <service>`
- **Description**: Generate an account for the specified service
- **Cooldown**: 7.5 minutes (normal) / 1 minute (premium)
- **Access**: Whitelisted users only
- **Features**: 
  - Auto-completion for available services
  - DM delivery for security
  - Stock tracking

#### `/p_gen <service>`
- **Description**: Premium generation with enhanced features
- **Cooldown**: 1 minute
- **Access**: Premium users only
- **Features**:
  - Priority generation
  - Enhanced account quality
  - Reduced cooldown

### 🛠️ **Management Commands**

#### `/restock <service> <amount>`
- **Description**: Announce a service restock
- **Access**: Whitelisted users only
- **Features**:
  - Automated announcements
  - Stock tracking updates

#### `/create_service <service>`
- **Description**: Create a new service for account generation
- **Access**: Whitelisted users only

#### `/stock [service]`
- **Description**: Check available account stock
- **Access**: All users
- **Features**:
  - Real-time stock display
  - Service-specific or global view

### 💎 **Premium Commands**

#### `/premium_key`
- **Description**: Generate a premium access key
- **Access**: Whitelisted users only
- **Features**:
  - Single-use keys
  - Secure generation

#### `/redeem_key <key>`
- **Description**: Redeem a premium key for premium access
- **Access**: All users
- **Features**:
  - Instant premium activation
  - Role assignment

### 🔧 **Utility Commands**

#### `/ping`
- **Description**: Check bot latency and status
- **Access**: All users
- **Features**:
  - Color-coded latency display
  - Real-time status check

---

## 💎 Premium System

### 🌟 **Premium Benefits**

- **⚡ Reduced Cooldown**: 1 minute instead of 7.5 minutes
- **📱 DM Generation**: Generate accounts via direct messages
- **🎯 Priority Access**: Access to `/p_gen` command

### 🎟️ **How to Get Premium**

1. **Get a Premium Key**: Ask a whitelisted user to generate one with `/premium_key`
2. **Redeem the Key**: Use `/redeem_key <your_key>` to activate premium
3. **Enjoy Premium**: Access all premium features immediately

---

## 🔒 Security Features

### 🛡️ **Access Control**
- **Server Whitelist**: Only authorized servers can use the bot
- **User Whitelist**: Individual user access control
- **Channel Restrictions**: Commands limited to specific channels
- **Auto-moderation**: Unauthorized messages automatically deleted

### 🔐 **Data Protection**
- **Secure DM Delivery**: Accounts sent privately to users
- **Key-based Premium**: Secure premium access system
- **No Data Logging**: User privacy protection

---

## 📊 Statistics

The bot tracks comprehensive statistics including:

- **Global Generation Count**: Total accounts generated
- **Service Statistics**: Per-service generation tracking
- **User Analytics**: Individual user usage statistics
- **Real-time Updates**: Live status updates with current stats

---

## 🆘 Support & Help

Need help with the bot? Have questions or issues?

**Contact me on Discord: `gxqk_secours`**

I'm here to help you with:
- ⚙️ Bot configuration and setup
- 🐛 Troubleshooting issues
- 💎 Premium access questions
- 🔧 General support and guidance

Don't hesitate to reach out!

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

<div align="center">

**Made with ❤️ by gxqk**

*If you find this project useful, please consider giving it a ⭐!*

</div>
