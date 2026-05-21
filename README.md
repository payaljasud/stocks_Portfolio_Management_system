# Stock Portfolio Manager

A Python-based application to manage your stock portfolio.
![image](https://github.com/user-attachments/assets/3e623115-cc1d-46a7-8a5c-90cc8a8fbada)

# Stock Portfolio Manager

A Python-based desktop application to manage and track your stock portfolio using Tkinter and SQLite.

[GitHub Repository](https://github.com/payaljasud/stocks_Portfolio_Management_system?utm_source=chatgpt.com)

# Features
- Track stock prices in real-time
- Manage trades (Bullish/Bearish)
- Set stop-loss and target prices
- SQLite database for storing data
- User-friendly Tkinter GUI

# Tech Stack
* Python
* Tkinter
* SQLite3
* Requests
* BeautifulSoup4

# Project Structure

```bash
stocks_Portfolio_Management_system/
│
├── main.py
├── stocks.db
├── README.md
└── requirements.txt
```

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/payaljasud/stocks_Portfolio_Management_system.git
cd stocks_Portfolio_Management_system
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install requests beautifulsoup4 certifi
```

---

## Run the Application

```bash
python main.py
```

---

## Application Functionalities

### Fetch Live Stock Price

Enter an NSE stock symbol and fetch the current market price directly from Google Finance.

### Add Trade

* Select trade type (Bullish/Bearish)
* Set:

  * Entry Price
  * Quantity
  * Stop Loss
  * Target Price

### Manage Portfolio

* View all trades in a table
* Edit existing trades
* Delete trades
* Monitor profit/loss percentage

---

## Database Schema

```sql
CREATE TABLE stocks (
    id INTEGER PRIMARY KEY AUTOINCREMENT,
    symbol TEXT UNIQUE,
    current_price REAL,
    entry_price REAL,
    quantity INTEGER,
    stop_loss REAL,
    target REAL,
    trade_type TEXT
);
```

## Future Improvements

* Stock charts and analytics
* Support for multiple stock exchanges
* Price alerts and notifications
* Cloud database integration
* Modern UI using CustomTkinter


## Contributing
Contributions, issues, and feature requests are welcome.
Feel free to fork the repository and submit a pull request.

# License
This project is open-source and available under the MIT License.




