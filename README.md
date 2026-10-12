# MarketPulse

MarketPulse is a full-stack trading-analytics platform that turns trading data into clear, actionable insights. It combines portfolio tracking, trade journaling, market news, and behavioural bias analysis in one application.

The platform helps users understand not only what they traded, but why they may be making certain trading decisions. It identifies behavioural patterns such as overtrading, loss aversion, and revenge trading, then provides practical guardrails to support better decision-making.

## Features

### Frontend
- **Watchlist:** Track selected symbols in one place.
- **Trade Journal:** Record entries, exits, profit/loss, and trade notes.
- **News View:** View market headlines and an economic calendar.
- **Settings:** Configure theme, accessibility, and privacy preferences.

### Backend
- **Chat Service:** Node.js/Express service for starting conversations with selected agents, sending messages, and attaching trading-history files.
- **Bias Detector API:** Accepts CSV or Excel uploads, validates and standardizes trade data, and returns structured behavioural insights.
- **Bias Analysis Engine:** Detects patterns including:
  - Overtrading
  - Loss aversion
  - Revenge trading

The bias detector returns summary statistics, bias cards with scores and triggers, recommendations, and chart-ready data.

## Tech Stack

- **Frontend:** TypeScript
- **Backend:** Node.js, Express
- **Analysis:** Python
- **Data Input:** CSV and Excel files
- **Other:** REST APIs, Git, GitHub

## Getting Started

### Prerequisites

Make sure you have the following installed:

- Node.js
- Python
- Git

### Installation

1. Clone the repository:

```bash
git clone [https://github.com/cole98ster/MarketPulse.git](https://github.com/cole98ster/MarketPulse.git)
cd MarketPulse
```

2. Install frontend dependencies:

```bash
npm install
```

3. Install backend dependencies:

```bash
cd backend
npm install
```

4. Install Python dependencies for the bias-detection service:

```bash
cd bias-detector
pip install -r requirements.txt
```

## Running the Application

Start the frontend:

```bash
npm run dev
```

Start the chat/backend service:

```bash
cd backend
npm start
```


## Usage

1. Open the application in your browser.
2. Add symbols to your watchlist.
3. Upload a CSV or Excel file containing your trading history.
4. Review the generated summary statistics and bias cards.
5. Use the recommendations to identify potential behavioural risks in your trading activity.

## Project Structure

```text
MarketPulse/
├── frontend/          # User interface and client-side application
├── backend/           # Node.js/Express chat and application services
├── bias-detector/     # Python API for trade-data analysis
└── README.md
```

## Roadmap

- Add persistent user accounts and saved trade history
- Improve charting and historical performance visualization
- Expand bias detection with additional trading-behaviour models
- Add automated testing for API endpoints and data validation
- Deploy the frontend and backend services


## License

This project is licensed under the [MIT License](LICENSE).

## Author

**Cole Neild**  
[LinkedIn](https://www.linkedin.com/in/cole-neild/)  
[GitHub](https://github.com/cole98ster)
