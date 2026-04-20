# XBOT

A simple Node.js script that uses the **Twit** library to search recent tweets containing a specific hashtag and automatically favorite them.

## Features
- Loads Twitter API credentials from a `.env` file via `dotenv`.
- Searches recent tweets for a configurable query (default: `#Reactjs`).
- Favorites each tweet found.

## Prerequisites
- **Node.js** (v24 or later)
- A Twitter developer account with **API Key**, **API Secret**, **Access Token**, and **Access Token Secret**.

## Setup
1. Clone the repository and navigate to the project folder.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file (use the provided template) and fill in your Twitter credentials:
   ```dotenv
   CONSUMER_KEY=your_consumer_key
   CONSUMER_SECRET=your_consumer_secret
   ACCESS_TOKEN=your_access_token
   ACCESS_TOKEN_SECRET=your_access_token_secret
   ```
4. Verify the configuration by running the optional test script:
   ```bash
   node test.js
   ```
   (It should print your Twitter screen name if the credentials are valid.)

## Running the Bot
```bash
node app.js
```
The script will search for recent tweets matching the query defined in `app.js` and favorite each one.

## License
MIT © 2026 sahiljadhav7
