# Telegram Crypto Price Bot

A Telegram bot that provides real-time price updates for Bitcoin (BTC) and Ethereum (ETH) using the CoinGecko API.

## Features

- Real-time BTC and ETH price updates every 30 seconds
- Price change percentage over 24 hours
- Simple subscription system with /start and /stop commands
- Error handling and logging

## Prerequisites

- Node.js 16 or higher
- A Telegram Bot Token (already configured)

## Setup

1. Clone the repository
   ```bash
   git clone https://github.com/YOUR_USERNAME/telegram-crypto-bot.git
   cd telegram-crypto-bot
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a .env file with your Telegram bot token:
   ```
   TELEGRAM_BOT_TOKEN=your_bot_token_here
   ```

4. Start the bot:
   ```bash
   npm start
   ```

## Deployment

### Railway.app Deployment

1. Fork this repository to your GitHub account
2. Go to [Railway.app](https://railway.app)
3. Create new project → Deploy from GitHub repo
4. Select the forked repository
5. Add environment variable:
   - TELEGRAM_BOT_TOKEN=your_bot_token_here
6. Railway will automatically deploy your bot

## Usage

1. Start a chat with the bot on Telegram
2. Send /start to subscribe to price updates
3. Send /stop to unsubscribe from updates

## Commands

- `/start` - Subscribe to price updates
- `/stop` - Unsubscribe from price updates

## Error Handling

The bot includes comprehensive error handling for:
- API failures
- Network issues
- Message delivery failures

Errors are logged to:
- console
- error.log (for errors)
- combined.log (for all logs)
