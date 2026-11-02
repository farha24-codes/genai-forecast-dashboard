# 📊 GenAI Sales Forecast Dashboard

A time-series sales forecasting dashboard that pairs **Prophet** forecasts with **Google Gemini**-generated, plain-English business insights. Instead of just showing a chart, the app explains what the forecast means so non-technical users can make decisions quickly.



---

## ✨ Features

- 📈 Forecasts future sales from historical data using Prophet
- 🔍 Visualizes trends, seasonality, and forecast confidence intervals
- 🤖 Generates plain-English business insights from the forecast using Gemini
- 🖥️ Interactive Streamlit interface, no coding needed to use it

## 🧠 How It Works

1. Historical sales data is loaded and cleaned
2. Prophet is trained on the data to model trend and seasonality
3. The model produces a forecast for the chosen future period
4. The forecast results are sent to Gemini as context
5. Gemini returns a clear, business-friendly summary shown next to the charts

## 🛠️ Tech Stack

| Area | Tools |
|------|-------|
| Language | Python |
| Forecasting | Prophet |
| GenAI | Google Gemini API |
| Dashboard | Streamlit |
| Data handling | Pandas |

## 📁 Project Structure

```
genai-forecast-dashboard/
├── app.py               # Streamlit app
├── requirements.txt     # Dependencies
├── data/                # Sales dataset(s)
├── screenshots/         # Dashboard images
└── README.md
```
<!-- Update the structure above to match your actual files -->

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/farha24-codes/genai-forecast-dashboard.git
   cd genai-forecast-dashboard
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   venv\Scripts\activate
   ```
   On macOS/Linux use `source venv/bin/activate`.

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Add your Gemini API key**

   Create a file named `.env` in the project root and add:
   ```
   GEMINI_API_KEY=your_api_key_here
   ```
   Get a free key at [Google AI Studio](https://aistudio.google.com/apikey).

5. **Run the app**
   ```bash
   streamlit run app.py
   ```
   Then open the local URL shown in your terminal (usually http://localhost:8501).

## 📊 Example Output

- Forecast chart with upper and lower confidence bounds
- Trend and seasonality components
- AI-generated summary, for example: *"Sales are expected to grow steadily over the next quarter, with a seasonal peak around year end..."*

## 🔮 Future Improvements

- Upload your own CSV for custom forecasting
- Compare multiple forecasting models
- Export insights as a PDF report
- Deploy on Streamlit Community Cloud

## 🔒 Note

Never commit your API key. Make sure `.env` is listed in `.gitignore`.
