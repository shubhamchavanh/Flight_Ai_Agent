✈️ AI-Powered Flight Booking Assistant

🚀 Overview

AI-Powered Flight Booking Assistant is a Streamlit-based web application that helps users search for flights using Firecrawl API for web scraping and OpenAI models for intelligent recommendations. The app retrieves flight data from Skyscanner and provides insights on the best travel options based on price, duration, and layovers.

🛠 Features

🔍 Search Flights by entering origin, destination, date, number of travelers, and cabin class.

🧠 AI-Powered Recommendations using OpenAI GPT models.

📊 Price & Duration Comparison for selecting the best flight.

🌍 Real-Time Web Scraping via Firecrawl API.

🎨 Streamlit UI for an interactive experience.

📥 Installation

1️⃣ Clone the Repository

git clone https://github.com/yourusername/ai-flight-booking.git
cd ai-flight-booking

2️⃣ Install Dependencies

pip install -r requirements.txt

3️⃣ Set Up API Keys

Create a .env file in the root directory and add your Firecrawl API Key and OpenAI API Key:

FIRECRAWL_API_KEY=your_firecrawl_api_key
OPENAI_API_KEY=your_openai_api_key

Or enter API keys directly in the Streamlit sidebar.

4️⃣ Run the App

streamlit run app.py

🎮 Usage

Enter Origin & Destination (IATA codes) 🏢✈️.

Select Departure Date 📅.

Choose Number of Travelers and Cabin Class 💺.

Click 🔍 Search Flights to fetch results.

![{F96DC901-B210-4E32-B2D1-537B1793EFAB}](https://github.com/user-attachments/assets/33b99e62-9ccc-4fa0-b470-de97baef692d)


View Flight Recommendations with price and duration insights.


🚀 Deployment Options

1️⃣ Streamlit Community Cloud (Easy & Free)

Push your code to GitHub.

Deploy via Streamlit Cloud.

2️⃣ Google Cloud Run

Create a Dockerfile:

FROM python:3.9
WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt
COPY . .
CMD ["streamlit", "run", "app.py", "--server.port=8080", "--server.address=0.0.0.0"]

Build & deploy:

gcloud builds submit --tag gcr.io/YOUR_PROJECT_ID/flight-agent
gcloud run deploy flight-agent --image gcr.io/YOUR_PROJECT_ID/flight-agent --platform managed --allow-unauthenticated

3️⃣ AWS EC2

Launch an EC2 instance and SSH into it:

ssh -i "your-key.pem" ubuntu@your-ec2-instance-ip

Install Python & Streamlit, then run:

streamlit run app.py --server.port=8080 --server.address=0.0.0.0

🔥 Future Enhancements

✅ Add Round-Trip Booking

🌎 Support for Multi-City Flights

📅 Implement Best Price Predictions

📜 License

This project is licensed under the MIT License.

🤝 Contributing

We welcome contributions! Feel free to open an issue or submit a pull request.

📧 Contact

For questions or support, contact your.email@example.com.

