# eco-gpt

# Eco gpt App Demo 🚀

This repo contains a Google Colab notebook that demonstrates a simple app for 🌿 Eco‑GPT Open‑Source Conservation Assistant .
Eco-GPT is a Streamlit app that answers scientific/ecological questions using:

CSV logs (e.g. sensor & wildlife observations)
Scientific PDFs (research notes, papers)

model backends:

   -Synthetic API (gpt-oss-120b)


It supports semantic retrieval with FAISS and cached embeddings so PDFs don’t re-index every run


## 🔗 Open in Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/frasfras/eco-gpt/blob/main/eco_gpt1_notebook.ipynb
)

Setup & Installation
1. Clone & install dependencies
## 📦 Requirements
   git clone https://github.com/yourname/eco-gpt.git
   cd eco-gpt
   
   upload eco-gpt1-notebook to Google Collab
   
2. Environment variables
   import os
   os.environ["SYNTHETIC_API_KEY"] = "your_api_key_here"
   # --------------------------
  # Setup API client
 
  client = openai.OpenAI(
   #api_key=os.environ.get("SYNTHETIC_API_KEY"),
     api_key="SYNTHETIC_API_KEY",

   # setup ngrok
   # Set your ngrok auth token (get free token from https://ngrok.com)

   NGROK_AUTH_TOKEN = "NGROK_AUTH_TOKEN"
   
4. Run in Google Colab with ngrok
   Run in Collab notebook  run all Cells. and Cell #5 "Run in Google Colab with ngrok".
   Click the printed URL to access the app.

   #Testing Instructions
Upload data

Upload a CSV in examples download (example: sample_logs.csv):
(Optional) Upload a scientific PDF with field notes or research. sample in examples folder

 Ask questions

In the text box, try:

CSV query:
“What animals were near stream #3?”

PDF query:
“Summarize findings about insect diversity.”
"What conditions favor jaguar sighting"

🌍 Eco-GPT Answer:
A jaguar was observed near stream #3 at 06:14:00 by cam_trap_01.

Install dependencies if running locally:
```bash
pip install -r requirements.txt
