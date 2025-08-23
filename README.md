<<<<<<< HEAD
# AI CryptoNewsletter Curator & Market Bot

This project aggregates, summarizes, and analyzes cryptocurrency newsletters using AI, and provides a Telegram bot for real-time market insights and news analysis.

## Project Overview

The AI CryptoNewsletter Curator is designed to provide users with comprehensive cryptocurrency market intelligence. It scrapes news from major crypto sources, performs sentiment analysis, and offers a Telegram bot interface for real-time interaction with market data and news insights.

## Core Functionalities

### News Processing Pipeline
- *Web Scraping*: Automatically scrapes news from major cryptocurrency sources (CoinDesk, CryptoSlate, Decrypt, CoinTelegraph)
- *Content Summarization*: Extracts and summarizes key information from news articles
- *Sentiment Analysis*: Uses VADER sentiment analysis to categorize news as positive, negative, or neutral
- *Image Generation*: Creates visual reports and summaries of market trends

### Telegram Bot Features
- *Universal News Analysis*: /news <cryptocurrency> - Get AI-powered analysis for any cryptocurrency (e.g., /news bitcoin, /news ethereum, /news cardano)
- *Live Price Charts*: /chart <ticker> - Get real-time price charts for any crypto or stock (e.g., /chart BTC-USD, /chart ETH-USD, /chart TSLA)
- *Conversational AI*: Ask natural language questions about markets and get intelligent responses
- *Gamification System*: Earn points and badges for using bot features
- *Session Management*: Privacy-focused user session handling with automatic cleanup

### Advanced Features
- *Groq AI Integration*: Uses Llama 3.1-8B for intelligent news analysis and conversational responses
- *Real-time Data*: Fetches live cryptocurrency prices using yfinance
- *News API Integration*: Supports NewsAPI.org for comprehensive news coverage
- *Context Awareness*: Maintains conversation context for more relevant responses
- *Multi-platform Support*: Works with any cryptocurrency worldwide

## Project Structure


market-bot/
├── src/
│   ├── main.py              # Main application entry point
│   ├── bot.py               # Telegram bot implementation
│   ├── scrapper.py          # Web scraping functionality
│   ├── summarizer.py        # News summarization
│   ├── sentiment_analysis.py # VADER sentiment analysis
│   ├── image_generator.py   # Report image generation
│   └── config.json          # Configuration for news sources
├── data/
│   ├── scraped_data.json    # Raw scraped news data
│   ├── summarized_data.json # Summarized news content
│   ├── sentiment_data.json  # Sentiment analysis results
│   └── final_report.json    # Final processed reports
├── images/                  # Generated report images
├── test_*.py               # Comprehensive test suite
└── README.md


## Setup Instructions

1. *Clone and navigate to the project:*
   bash
   git clone <repository-url>
   cd market-bot
   

2. *Install required dependencies:*
   bash
   pip install python-telegram-bot yfinance requests beautifulsoup4 nltk groq python-dotenv matplotlib pandas pillow
   

3. *Set up environment variables* in a .env file:
   
   TELEGRAM_BOT_TOKEN=your_telegram_bot_token
   GROQ_API_KEY=your_groq_api_key
   NEWS_API_KEY=your_newsapi_org_key  # Optional: Get from https://newsapi.org/
   

4. *Run the Telegram bot:*
   bash
   python bot.py
   

5. *Run individual components:*
   bash
   # Run web scraper
   python src/scrapper.py
   
   # Run sentiment analysis
   python src/sentiment_analysis.py
   
   # Run tests
   python test_universal_news.py
   

## Usage Examples

### Telegram Bot Commands:
- /start - Welcome message and command overview
- /news bitcoin - Get AI analysis of Bitcoin news
- /chart ETH-USD - Get Ethereum price chart
- /points - Check your points and badges
- Just type any cryptocurrency name (e.g., "BTC", "ethereum") to get a chart

### Natural Language Interaction:
- "What's happening with Bitcoin today?"
- "Should I invest in Ethereum?"
- "Show me Cardano news"
- "How is the crypto market doing?"

## API Keys Required

- *Telegram Bot Token*: Get from @BotFather on Telegram
- *Groq API Key*: Free tier available at https://console.groq.com/
- *NewsAPI Key* (Optional): Free tier available at https://newsapi.org/

## Testing

The project includes comprehensive test suites:
- test_universal_news.py - Tests news functionality for various cryptocurrencies
- test_enhanced_bot.py - Tests advanced bot features
- test_indian_news.py - Tests region-specific news
- test_news.py - General news functionality tests

Run tests with:
bash
python test_universal_news.py


## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- NewsAPI.org for providing news data
- Groq for AI inference capabilities
- Telegram for bot platform
- yfinance for market data
- The open-source community for various libraries and tools
=======

>>>>>>> 6c9c50d184c2afa5995ae0d83c74ce724b1fef98
