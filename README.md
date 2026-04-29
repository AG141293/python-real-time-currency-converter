# 💱 Python Currency Converter using Fixer API

A real-time currency converter built in Python using the Fixer API that allows users to convert between multiple global currencies using live exchange rates.

## 📌 Overview
This project fetches the latest foreign exchange rates from the Fixer API and performs real-time currency conversion based on user input.

It is a simple command-line application demonstrating:

- API integration in Python
- JSON data handling
- Currency conversion logic
- Error handling and validation
- Interactive CLI design

---

## 🚀 Features

✅ Real-time exchange rates using Fixer API  
✅ Supports multiple international currencies  
✅ Command-line based interactive converter  
✅ Currency lookup list (`SHOW` command)  
✅ Invalid input and error handling  
✅ Easy to run in Python or Google Colab

---

## 🛠 Tech Stack

- Python
- Requests
- JSON
- Fixer API
- Google Colab / Jupyter Notebook

---


## 🔑 API Setup

This project uses the Fixer API.

Get a free API key from:

https://fixer.io

Replace:

```python
YOUR_API_KEY
```

with your own API key.

### Better Security (Recommended)
Store the key using environment variables instead of hardcoding:

```python
import os
api_key = os.getenv("FIXER_API_KEY")
```

---

## ▶️ Run the Project



## 💻 Usage

Input format:

```bash
amount FROM_CURRENCY TO_CURRENCY
```

Example:

```bash
100 USD INR
```

Output:

```bash
100 USD = 8334.21 INR
```

---

## 📋 Available Commands

Show supported currencies:

```bash
SHOW
```

Quit program:

```bash
Q
```

---

## 🧠 How Conversion Works

Conversion formula used:

```text
Converted Amount =
Amount × (Target Currency Rate / Source Currency Rate)
```

Example:

```text
100 USD → INR
100 × (INR rate / USD rate)
```

---

## 🔍 Sample Code

```python
amount = round(
    qty * fx[toC] / fx[fromC],
    2
)
```

---

## ⚠ Error Handling

The program handles:

- Invalid currency codes
- Incorrect input format
- API response issues
- Missing exchange rates

Example:

```bash
You seem to have inputted wrongly, retry!
```

---

## 🌍 Supported Currencies

Includes major currencies such as:

- USD
- EUR
- INR
- GBP
- JPY
- AUD
- CAD
- BTC

and many more.

Use:

```bash
SHOW
```

to see full list.

---

## 📈 Future Improvements

Possible enhancements:

- GUI version using Tkinter/Streamlit
- Flask web app deployment
- Historical exchange rate charts
- Currency trend visualization
- Support for crypto conversions
- Unit tests and modular structure

---

## 🎯 Learning Outcomes

This project helped practice:

- Working with REST APIs
- Parsing JSON data
- Python functions and recursion
- Exception handling
- Building interactive CLI tools

---

## 🤝 Contributing

Contributions and suggestions are welcome.

Fork the repository and submit a pull request.

---

## 📜 License

This project is open-source under the MIT License.

---

## 👩‍💻 Author

Ankita Ghosh

If you found this project useful, feel free to star ⭐ the repository.
