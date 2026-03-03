💱 Currency Exchange Rate Converter

A responsive web application that provides real-time currency conversion using live exchange rate data. Built with vanilla JavaScript (ES6+), this project demonstrates API integration, asynchronous programming, and dynamic DOM manipulation.

---

📌 Overview

The Currency Exchange Rate Converter allows users to convert amounts between international currencies instantly. Exchange rates are fetched from a public exchange rate API and updated dynamically without requiring a backend server.

This project is ideal for demonstrating frontend development fundamentals and working with external APIs.

---

✨ Features

* 🌍 Real-time currency conversion
* 🔄 Support for multiple global currencies
* ⚡ Instant calculation using Async/Await
* 📱 Fully responsive design
* 🧮 Dynamic currency selection
* 🛡️ Error handling for API failures
* 🚀 Lightweight and fast (no frameworks)

---

🛠️ Tech Stack

* **HTML5** – Semantic structure
* **CSS3** – Responsive styling
* **JavaScript (ES6+)** – Application logic
* **Fetch API** – API calls
* **Exchange Rate API** – Live currency data

---

📂 Project Structure

```
currency-exchange-rate-converter/
│
├── index.html      # Application structure
├── style.css       # Styling and layout
├── script.js       # API logic and DOM manipulation
└── README.md       # Project documentation
```

---

🚀 Getting Started

1️⃣ Clone the Repository

```bash
git clone https://github.com/Amy-source/CurrencyConverter.git
```

2️⃣ Navigate to Project Directory

```bash
cd CurrencyConverter
```

3️⃣ Open in Browser

Simply open `index.html` in your preferred browser.

No build tools or dependencies required.

---

🔗 API Integration

The application fetches exchange rates dynamically using a free public API.

Example implementation:

```javascript
async function getExchangeRate(from, to, amount) {
    const url = `https://api.exchangerate.host/latest?base=${from}&symbols=${to}`;
    
    const response = await fetch(url);
    const data = await response.json();

    const rate = data.rates[to];
    return amount * rate;
}
```

---

📊 How It Works

1. User selects base currency.
2. User selects target currency.
3. User enters amount.
4. Application fetches latest exchange rate.
5. Converted value is displayed instantly.

---

🎯 Learning Objectives

This project demonstrates:

* REST API consumption
* Asynchronous JavaScript (Async/Await)
* Fetch API usage
* DOM manipulation
* Event handling
* Clean UI design principles

---

📈 Future Improvements

* Historical exchange rate charts
* Currency swap button
* Dark mode support
* Loading indicators
* Accessibility improvements
* Unit testing implementation

---
🌐 Deployment

This project can be deployed using:

* GitHub Pages
* Netlify
* Vercel

---

