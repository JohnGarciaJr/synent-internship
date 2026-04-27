# Task 1 — Weather App (Intermediate Python Project)

## 📌 Overview
This project is part of the **Synent Technologies Python Development Internship**.  
The goal of Task‑1 is to build a simple, modular **Weather Application** that retrieves real‑time weather data using a public API and displays it in a clean, readable format.

This task demonstrates:
- API requests  
- JSON parsing  
- Error handling  
- Environment variable usage  
- Modular Python scripting  

---

## 🧠 Features
- Fetches current weather for any city  
- Uses the OpenWeatherMap API  
- Handles invalid city names and network errors  
- Reads API key from a `.env` file  
- Clean, modular code structure  

---

## 🛠️ Tech Stack
- Python 3.x  
- `requests`  
- `python-dotenv`  
- OpenWeatherMap API  

---

## 📦 Project Structure

```
task-1/
│── README.md
└── src/
└── weather.py
```

---

## 🔑 Setup Instructions

### 1️⃣ Install dependencies
Run this inside the `task-1` folder:

```
pip install -r requirements.txt
```

### 2️⃣ Create a `.env` file  
Inside `task-1/src/`, create a file named `.env`:

```
API_KEY=your_openweathermap_api_key_here
```

### 3️⃣ Run the script

```
python src/weather.py
```

You will be prompted to enter a city name.

---

## 🌦️ Example Output

Weather for Houston, US

Temperature: 82°F
Feels Like: 85°F
Condition: Clear sky
Humidity: 60%
Wind Speed: 4.5 mph

---

## 🧪 Error Handling Examples

- Invalid city  
- Missing API key  
- Network issues  
- API downtime  

The script prints friendly, readable error messages.

---

## 📸 Screenshots (Optional)
Add screenshots of your terminal output here.

---

## ✅ Status
✔️ Task‑1 in progress  
✔️ README created  
⬜ Code completed  
⬜ Testing  
⬜ Final submission

---
