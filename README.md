# Paper-Trading-Website
**Paper Trading Website**: A Django website to practice stock trading with virtual funds. Features include stock search, dynamic stock price charts, a history of user trades, real-time data integration, and user authentication. Perfect for testing trading strategies without financial risk.

---

## Features

- **Stock Search**: Search and add stocks by symbol.
- **Portfolio Management**: Track and manage your virtual stock holdings.
- **Interactive Charts**: View dynamic charts of stock price trends.
- **Real-Time Data**: Powered by Alpaca's API for the latest stock information.
- **User Authentication**: Secure signup and login to save your portfolio and preferences.

---

## Installation

### Prerequisites
- Python 3.9+
- Django 4+
- Alpaca API Key and Secret
- Git

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/newoatsoca/paper-trading-simulator.git
   cd paper-trading-simulator
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up the `.env` file with your Alpaca API credentials:
   ```env
   ALPACA_API_KEY=your_api_key
   ALPACA_SECRET_KEY=your_secret_key
   DEBUG=True
   ```

5. Apply database migrations:
   ```bash
   python manage.py migrate
   ```

6. Start the development server:
   ```bash
   python manage.py runserver
   ```

Visit `http://127.0.0.1:8000/` to view the app.

---

## Usage

### Stocks Page
The Stocks Page displays available stocks and a search bar for adding new stocks to your watchlist.

### Portfolio
View your balance, active stock holdings, and their total values.

### Stock Details
Click on a stock to view detailed information, including price trends and interactive charts.

### Authentication
Sign up or log in to save your portfolio and preferences securely.

---

## Technologies Used

- **Frontend**: HTML, Django Templates
- **Backend**: Django, Python
- **Database**: SQLite (default; can be replaced with PostgreSQL or MySQL)
- **API**: Alpaca Market Data API
- **Charts**: Plotly for interactive data visualization

---

## License
This project is licensed under the MIT License.

---

## IDE
This project was made with JetBrains' PyCharm

