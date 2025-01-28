# E-commerce Competitor Strategy Dashboard

## What’s This Project About?
This project is all about creating a powerful *E-commerce Competitor Strategy Dashboard* to help businesses stay ahead of the game. The idea is to analyze competitor data, predict trends, and come up with actionable strategies to improve pricing, promotions, and customer satisfaction. It uses tools like web scraping, machine learning, and AI to deliver clear, useful insights.

---

## Key Features

### 1. Collecting Competitor Data
- The dashboard scrapes daily competitor data like pricing, discounts, and reviews (from platforms like Amazon) using BeautifulSoup.
- All this data is saved in two handy CSV files:
  - **competitor_data.csv**: Includes product prices, discounts, and dates.
  - **reviews.csv**: Stores customer reviews for each product.

### 2. Analyzing Customer Sentiment
- Customer reviews are analyzed for sentiment (positive, negative, or neutral) using Hugging Face’s NLP tools.
- These results are shown in a clear, interactive bar chart made with Plotly.

### 3. Predicting Discounts
- A Random Forest model predicts discounts based on product prices.
- An ARIMA model forecasts future discounts for the next five days, giving you a sneak peek at what’s coming.

### 4. Strategy Recommendations
- OpenAI’s API is used to generate smart strategies based on:
  - Competitor data and predicted trends.
  - Insights from customer sentiment analysis.

### 5. Slack Integration
- Any strategies generated are sent directly to a Slack channel so stakeholders can act quickly.

### 6. Interactive Dashboard
- Built with Streamlit, the dashboard lets users:
  - Select a product and explore its data.
  - View competitor analysis, discount predictions, and sentiment trends.
  - Access detailed, AI-generated recommendations.

---

## How It Works

### Data Collection
- Predefined product URLs are scraped using BeautifulSoup to get prices, discounts, and reviews.

### Data Preprocessing
- Prices and discounts are cleaned up and turned into usable numbers.
- Dates are formatted properly for time-series forecasting.

### Machine Learning Models
- **Random Forest Regressor** predicts discounts based on historical data.
- **ARIMA** forecasts trends for discounts over the next five days.

### Sentiment Analysis
- Hugging Face's sentiment analysis model determines whether customer reviews are positive, negative, or neutral.
- The results are visualized as an easy-to-understand bar chart.

### OpenAI’s API for Strategy
- The API generates tailored recommendations for optimizing pricing, promotions, and customer satisfaction based on the data.

---

## Getting Started

### What You’ll Need:
- **Python 3.8 or above**
- Libraries like:
  - pandas, numpy, streamlit, plotly, requests, beautifulsoup4, scikit-learn, statsmodels, transformers
- API keys for:
  - OpenAI (Groq API)
  - Slack Webhook

### Setup Instructions:
1. **Clone the repository:**
   ```bash
   git clone https://github.com/username/repository-name.git
   cd ecommerce-strategy-dashboard
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Add your API keys:**  
   Open the `API_KEY.py` file and paste:
   ```python
   GROQ_API_KEY = "your-groq-api-key"
   SLACK_WEBHOOK_API_KEY = "your-slack-webhook-key"
   ```

4. **Scrape competitor data:**
   ```bash
   python scraper.py
   ```

5. **Run the dashboard:**
   ```bash
   streamlit run app.py
   ```

---

## What You’ll See

### The Dashboard:
- **Competitor Analysis**: See prices, discounts, and trends.
- **Sentiment Analysis**: Explore customer sentiment with interactive visuals.
- **Discount Forecasting**: Get predictions for the next 5 days.
- **Strategy Recommendations**: AI-driven suggestions for pricing and promotions.

### Slack Notifications:
- Important strategies sent directly to your Slack channel for easy access.

---

## What’s Next?
Here’s how we plan to make this even better:
- Add scraping support for more e-commerce platforms.
- Use more advanced NLP models for deeper sentiment analysis.
- Enable real-time data updates for even fresher insights.

---

## Visuals
Take a look at some of the screenshots from the dashboard below:

![Screenshot 1](https://github.com/SANIA1A1216/E-commerce-competitor-Analysis/blob/main/Screenshot-1.png)
![Screenshot 2](https://github.com/SANIA1A1216/E-commerce-competitor-Analysis/blob/main/Screenshot%202025-01-28%20153414.png)
![Screenshot 3](https://github.com/SANIA1A1216/E-commerce-competitor-Analysis/blob/main/Screenshot%202025-01-28%20175337.png?raw=true)
![Screenshot 4](https://github.com/SANIA1A1216/E-commerce-competitor-Analysis/blob/main/Screenshot%202025-01-28%20175951.png?raw=true)

---

## License
This project is open-source and licensed under the MIT License.

---

## Acknowledgments
Big thanks to:
- **Streamlit** for the interactive dashboard framework.
- **Hugging Face** for making sentiment analysis a breeze.
- **BeautifulSoup** for web scraping.
- **OpenAI** for strategy generation.

---

Let me know if you’d like more edits or have specific points you’d like to highlight!
