# eco-gpt

# Eco gpt App Demo 🚀

This repo contains a Google Colab notebook that demonstrates a simple app for 🌿 Eco‑GPT Open‑Source Conservation Assistant .
Eco-GPT is a Streamlit app that answers scientific/ecological questions using:<br/>

CSV logs (e.g. sensor & wildlife observations)
Scientific PDFs (research notes, papers) <br/>

 model backends used:
    
  # -Synthetic API (gpt-oss-120b) 


It supports semantic retrieval with FAISS and cached embeddings so PDFs don’t re-index every run


## 🔗 Open in Colab
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/frasfras/eco-gpt/blob/main/eco_gpt1_notebook.ipynb
)

Setup & Installation
1. Clone & install dependencies
## 📦 Requirements
   git clone https://github.com/frasfras/eco-gpt.git
   cd eco-gpt

   Click Open in Collab button above  
   Or upload eco-gpt1-notebook to Google Collab
   
2. ##  Environment variables
   
   Setup API client https://synthetic.new    <br/>
   use provided api key
   ##api_key= ("SYNTHETIC_API_KEY"), <br/>
  client = openai.OpenAI(
     api_key="SYNTHETIC_API_KEY",
   <br/>
3. ## setup ngrok
    Set your ngrok auth token (get token from https://ngrok.com)

   NGROK_AUTH_TOKEN = "NGROK_AUTH_TOKEN"
   
4. ## Run in Google Colab with ngrok <br/>
   Run in Collab notebook  run all Cells. and Cell #4 "Run in Google Colab with ngrok". 
   Click the printed URL below to access the app.
##
5. ## Testing Instructions
  Upload data

  Upload a CSV in examples download (example: sample_logs.csv): 
  eco-gpt/examples
- Upload a scientific PDF with field notes or research. sample in eco-gpt/examples folder

 Ask questions

In the text box, try:

CSV query:
“What animals were near stream #3?”

PDF query:
“Summarize findings about insect diversity.”
"What conditions favor jaguar sighting"
“What happens to the jaguar population if logging is halted for the next five years?”

🌍 Eco-GPT Answer:
A jaguar was observed near stream #3 at 06:14:00 by cam_trap_01.

Install dependencies if running locally:
```bash
