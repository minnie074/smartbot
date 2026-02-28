# SMART BOT 🤖

A simple and intelligent chatbot powered by Google's Gemini AI, built with Streamlit.

## Features

- 💬 Interactive chat interface
- 🚀 Powered by Google Gemini 2.5 Flash
- 🎨 Clean and modern UI with Streamlit
- ⚡ Fast and responsive

## Demo

Ask any question and get intelligent responses from Gemini AI!

## Prerequisites

- Python 3.8 or higher
- Google Gemini API Key ([Get it here](https://makersuite.google.com/app/apikey))

## Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd chat-main
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**
   
   Create a `.env` file in the root directory:
   ```bash
   cp .env.example .env
   ```
   
   Then add your Google Gemini API key to `.env`:
   ```
   GOOGLE_API_KEY=your_api_key_here
   ```

4. **Run the application**
   ```bash
   streamlit run app.py
   ```

5. **Open your browser**
   
   Navigate to `http://localhost:8501`

## Deployment on Streamlit Cloud

1. Push your code to GitHub (ensure `.env` is in `.gitignore`)
2. Go to [Streamlit Cloud](https://streamlit.io/cloud)
3. Connect your GitHub repository
4. Add your API key in **Settings → Secrets**:
   ```toml
   GOOGLE_API_KEY = "your_api_key_here"
   ```
5. Deploy!

## Project Structure

```
chat-main/
├── app.py              # Main application file
├── requirements.txt    # Python dependencies
├── .env               # Environment variables (not in git)
├── .env.example       # Example environment file
├── .gitignore         # Git ignore rules
└── README.md          # This file
```

## Technologies Used

- **Streamlit** - Web framework
- **Google Generative AI** - Gemini AI API
- **Python-dotenv** - Environment variable management

## Usage

1. Enter your query in the input box
2. Click "Ask your Query" button
3. Get intelligent responses from Gemini AI

## Security Note

⚠️ **Never commit your `.env` file to GitHub!** Your API key should remain private.

## License

This project is open source and available under the MIT License.

## Contributing

Contributions, issues, and feature requests are welcome!

## Author

Created with ❤️ using Streamlit and Google Gemini AI

---

**Note:** This project uses the `google-generativeai` package. Consider migrating to `google.genai` package for long-term support.
