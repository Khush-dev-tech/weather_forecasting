Weather Forecast
---
markdown
# 🌤 Weather Forecast Generator + Dashboard
This project generates synthetic weather data, uploads it to Google Sheets, and visualizes it with a **Supaboard-style dashboard** built using **Streamlit**.
---
## 🚀 Features

- ✅ Generate 100 rows of synthetic weather data across 4 specific dates
- ✅ Upload the data to **Google Sheets** via Google API
- ✅ Visualize data live on a **Streamlit dashboard**
- ✅ Clean UI with dynamic line charts for key weather metrics

---

## 🧩 Technologies Used

- Python 🐍
- Pandas 📊
- Google Sheets API (via `gspread` + `oauth2client`) 📄
- Streamlit (for the dashboard) 📈

---

## 📁 Project Structure


weather-dashboard/
├── weather_data_generator.py               # Script to generate & upload weather data
├── dashboard/
│   └── app.py                              # Streamlit Supaboard-style dashboard
├── credentials/
│   └── weather-forecast-456611-xxxx.json   # Google API credentials (replace with your file)
├── requirements.txt                        # Project dependencies
└── README.md                               # You’re reading it :)


---

## 🔧 Setup Instructions

### 1. Clone the Repository

bash
git clone https://github.com/your-username/weather-dashboard.git
cd weather-dashboard


### 2. Create `credentials/` Folder and Add Credentials

Place your Google Sheets service account JSON key in a folder named `credentials/`.  
Make sure the file is named something like:


credentials/weather-forecast-456611-xxxx.json


> 💡 [Create service account + enable Sheets API →](https://docs.gspread.org/en/latest/oauth2.html)

### 3. Install Python Dependencies

bash
pip install -r requirements.txt


---

## ⚙ How to Run

### Generate & Upload Weather Data

bash
python weather_data_generator.py


This script:
- Generates 100 rows of synthetic weather data
- Cycles through 4 specific dates (`2025-04-10` to `2025-04-13`)
- Uploads it to your `weather-forecast` Google Sheet

### Start the Dashboard

bash
streamlit run dashboard/app.py


Your live dashboard is now viewable at `http://localhost:8501/`

---

## 📊 Dashboard Overview

- **📅 Date-wise weather entries**
- **📈 Line charts** for Temperature and Humidity trends
- **📋 Full interactive table** of weather data
- **🌀 Minimalist UI**, inspired by Supaboard-style design

---

## ✅ Sample Output
![image](https://github.com/user-attachments/assets/de6e9b0c-860c-4844-bfa0-d6a3e1788c63)


![image](https://github.com/user-attachments/assets/6efa534c-5155-476e-9a73-b96a17dc1cfa)

From the console:

✅ Sample Output:
         Date  MinTemp  MaxTemp  Temp  Humidity  Pressure
0  2025-04-12      7.2     23.8  21.4        48    1015.8
1  2025-04-13      9.3     28.1  25.2        33    1007.2
...


In the dashboard:

- A line chart of Temperature & Humidity over 4 days
- Clean data table, with automatic refresh on rerun

---

## 📦 Requirements


pandas
gspread
oauth2client
streamlit
---

---
 🧠 Notes

- Make sure your *Google Sheet* is named weather-forecast
- Share the Sheet with your *service account email*
- The dashboard fetches live data directly from Google Sheets

---
✨ Credits
Inspired by Supaboard UI philosophy — clean, simple, functional.
---
Build by: Khush Aghera
          Sakshi Shelke
          Yash Saxena

