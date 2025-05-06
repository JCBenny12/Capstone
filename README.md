

# Project55 - Enhanced Chatbot Application

This project is an advanced chatbot application built using Streamlit, designed to interact with a Language Model (LLM) running on Google Colab via an Ngrok HTTP endpoint. The application now includes support for multiple LLM models, OpenCV, and OpenAI Whisper for enhanced functionality.

---

## Features
- **Chat Interface**: Clean and intuitive chat interface using Streamlit's `st.chat_message`.
- **Real-Time Streaming**: Bot responses are streamed for a seamless interaction experience.
- **Session State**: Maintains conversation history during the session.
- **Multi-Model Support**: Interact with multiple LLM models.
- **Computer Vision**: Integrated OpenCV for image processing.
- **Audio Processing**: Integrated OpenAI Whisper for audio processing.

---

## Requirements
- Python 3.8 or higher
- Streamlit
- Requests library
- OpenCV
- OpenAI Whisper

---

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/theOneAndOnlyOne/Project55.git
   cd gui_streamlit
   ```

2. **Create a Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate   # On macOS/Linux
   venv\Scripts\activate      # On Windows
   ```

3. **Install Required Modules**
   ```bash
   pip install -r requirements.txt
   ```

   If a `requirements.txt` does not work, you can manually install the required modules:
   ```bash
   pip install streamlit requests opencv-python openai-whisper
   ```
---

## Running the Application

1. Ensure Google Colab notebook is running in the background ([https://colab.research.google.com/drive/12E4xQuTRycC9nyvbi3U0K7OfoWdA9pWA?usp=sharing](https://colab.research.google.com/drive/12E4xQuTRycC9nyvbi3U0K7OfoWdA9pWA?usp=sharing))

2. Ensure ngrok tunnel is active (https://top-mule-adequately.ngrok-free.app)

3. Start the Streamlit server:
   ```bash
   streamlit run app.py 
   python -m streamlit run app.py # Alternatively
   ```

2. Open your browser and navigate to localhost, which is likely:
   ```
   http://localhost:8501
   ```

3. Interact with the chatbot in the provided interface.

---

## File Structure

```
colab_notebook/
│
└── HarryV1.ipynb          # Python notebook containing Ollama instance running LLM--will be run on Colab or similar application

gui_streamlit/             # Will also contain future Computer Vision and Audio 
│
├── app.py                 # Main application file
├── requirements.txt       # List of Python dependencies
└── .streamlit/            # Streamlit configuration folder (optional)
    └── secrets.toml       # API key storage (if required)
```

---

## Troubleshooting

- **Streamlit not found**: Ensure the virtual environment is activated and run `pip install streamlit`.
- **API Error**: Verify the Ngrok URL and ensure it is accessible.
- **JSON Parsing Error**: Check the Ollama API response format for inconsistencies.
- **OpenCV Error**: Ensure OpenCV is installed correctly and compatible with your Python version.
- **Whisper Error**: Ensure OpenAI Whisper is installed and configured properly.

---

## Future Enhancements
- Further enhance the UI with custom theming.
- Add more advanced NLP features.
- Improve performance and scalability.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.
