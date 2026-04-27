# 📘 Task 2 — Web Scraper (Books to Scrape)

## 📌 Overview
This project is part of the **Synent Technologies Python Development Internship**.  
The goal of Task 2 is to build a **fully interactive web scraper** that extracts book data from the *Books to Scrape* website using:

- `requests`
- `BeautifulSoup`
- Clean, modular Python functions
- A user‑friendly CLI interface

The scraper supports category selection, pagination, JSON/CSV export, and previewing results.

---

## 🚀 Features

### ✅ Interactive Category Selection
- Automatically scrapes all available categories from the homepage  
- Displays category names **with book counts**  
- Supports selecting by **number or name**  
- Prevents selecting empty categories  

### ✅ Accurate Pagination Handling
- Loads `index.html` for page 1  
- Loads `page-2.html`, `page-3.html`, etc. for additional pages  
- Ensures **all books** in a category are scraped  

### ✅ Flexible Output Options
After scraping, users can choose:

1. **JSON export**  
2. **CSV export**  
3. **Preview 5 Results Only (No Export)**  

If preview is selected, the user is then asked:

> “Would you like to export the full results?”

### ✅ Looping Workflow
After each scrape, the user can:

- Scrape another category  
- Exit the program cleanly  

### ✅ Refactored, Modular Code
The project uses helper functions for:

- Category selection  
- Scraping  
- Exporting  
- Previewing  
- Loop control  

This keeps the code clean, readable, and maintainable.

---

## 🧩 Project Structure

```
task-2/
│
├── scraper.py          # Main scraper logic
├── README.md           # Documentation (this file)
├── requirements.txt    # Dependencies (requests, beautifulsoup4)
└── exports/            # (Optional) Folder for saved JSON/CSV files
```


---

## 🛠️ Installation

### 1. Install dependencies
```bash
pip install -r requirements.txt
```

### 2. Run the scraper
```bash
python scraper.py
```
If in terminal, use
```bash
python src\scraper.py
```

---
## 🧠 How It Works

## 1. Load Categories
The scraper fetches all categories from the homepage and displays them like:
```
37. Contemporary (3 books)
38. Spirituality (6 books)
...
```

## 2. Use Select a Category
You can enter:

- The category number

- The category name (case‑insensitive)

## 3. Scraping Begins
The scraper:

- Loads page 1 (index.html)

- Loads additional pages (page-2.html, etc.)

Extracts:

- Title

- Price

- Availability

## 4. Choose Output Format
```
1. JSON
2. CSV
3. Preview 5 Results Only (No Export)
```

## 5. Optional Export After Preview
If preview is chosen, the user can still export afterward.

## 6. Loop or Exit
The user can scrape another category or exit.

---

## 📄 Example Output (Preview Mode)
```
Scraped 11 books from Philosophy

{'title': "Sophie's World", 'price': '£15.94', 'availability': 'In stock'}
{'title': 'The Death of Humanity...', 'price': '£58.11', 'availability': 'In stock'}
{'title': 'The Stranger', 'price': '£17.44', 'availability': 'In stock'}
{'title': 'Proofs of God...', 'price': '£54.21', 'availability': 'In stock'}
{'title': 'Kierkegaard...', 'price': '£47.13', 'availability': 'In stock'}
```

---

## 🧪 Error Handling
The scraper gracefully handles:

- Network errors

- Missing pages

- Invalid category input

- Empty categories

- Unexpected HTML changes

## 🧼 Code Quality
This project follows:

- PEP‑8 formatting

- Modular function design

- Clear separation of concerns

- Readable CLI output

## 📚 Dependencies
requests

beautifulsoup4

## 🏁 Conclusion
This task demonstrates:

- Web scraping fundamentals

- Pagination handling

- CLI design

- Data export workflows

- Clean, maintainable Python architecture
