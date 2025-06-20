
# LoanMate

Introducing a RAG-powered chatbot designed for accurate, document-driven answers on Indian loan schemes. This solution integrates LangChain with the ChatGroq (LLaMA 3) large language model. It leverages FAISS and Google AI embeddings to facilitate highly effective semantic search. Users benefit from instant responses, clear transparency (showing document similarity for answers), and a user-friendly interface built with Streamlit.



## Run Locally

Clone the project

```bash
  git clone https://github.com/dip011/loan-advisor-bot.git loan-advisor-bot
```

Go to the project directory

```bash
  cd loan-advisor-bot
```

Create and activate the virtual environment

```bash
  python -m venv venv

  source venv/bin/activate
```

Install all the required dependencies

```bash
  pip install -r requirements.txt 
```
Add PDF documents

Create a folder named ```data/``` in the root directory and place all the loan-related PDF documents from different banks inside it. These documents will be used by the chatbot for question answering.

```bash
  loan-advisor-bot/
├── data/
│   ├── hdfc_home_loans.pdf
│   ├── icici_loan_terms.pdf
│   └── ...


```

### Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`GROQ_API_KEY = your_groq_api_key_here`

`PDF_DATA_DIR = Path_ to_ the_ folder_ containing_ all_ loan-related_ PDF_ documents_ from_ different_ banks`

##
### Run the Application

```bash
  streamlit run app.py
```


