💼 Autonomous Investment Research Agent
🧠 Overview
This project builds an autonomous Investment Research Agent capable of analyzing public companies using financial data, news sentiment, macroeconomic indicators, and regulatory filings. The agent dynamically plans its research steps, routes content to specialized modules, evaluates its own output, and learns across runs.

👥 Team Members
Name	Role	Focus Area
Senthil Arasu T	Financial Data Analyst	Yahoo Finance, earnings, valuation
Member 2	News & Sentiment Analyst	NewsAPI/Kaggle, prompt chaining
Member 3	Agent Architect & Evaluator	Routing, memory, evaluator–optimizer
🧩 Key Features
RetrievalQA: Answers open-domain questions using grounded financial data

Prompt Chaining: Ingest → Preprocess → Classify → Extract → Summarize (for news)

Routing: Directs content to specialized analyzers (e.g., earnings, macro, sentiment)

Evaluator–Optimizer: Evaluates quality of analysis and refines using feedback

Memory System: Stores notes and insights across runs for continuous learning

📚 Datasets & APIs Used
yfinance – Stock prices, financial statements

NewsAPI / Kaggle Financial News – Market sentiment and headlines

FRED API – Macroeconomic indicators

SEC EDGAR – Company filings (10-K, 10-Q)

Alpha Vantage (optional) – Technical indicators and global assets

🏗️ Project Structure
Code
investment-research-agent/
│
├── README.md                  # Project overview and instructions
├── requirements.txt           # Python dependencies
├── data/                      # Raw and processed datasets
├── notebooks/                 # Exploratory notebooks by team members
├── src/                       # Core source code
│   ├── agent/                 # Planning, routing, evaluation, memory
│   ├── pipelines/            # Prompt chaining workflows
│   ├── retrievers/           # FAISS or vector DB setup
│   └── utils/                # Helpers and configs
├── tests/                    # Unit tests and evaluation scripts
└── docs/                     # Architecture diagrams, team notes
🚀 Getting Started
Clone the repository

Install dependencies:

bash
pip install -r requirements.txt
Run exploratory notebooks in /notebooks to test individual modules

Integrate modules into the agent workflow in /src/agent

🧪 Evaluation Criteria
Accuracy and relevance of answers

Grounding in retrieved financial data or news

Agent’s ability to reflect and refine its output

Collaboration across modules and memory usage

📅 Milestones
Week	Goal
1	Set up repo, assign roles, load datasets
2	Build retrieval + financial analysis
3	Implement news pipeline + routing
4	Add evaluator–optimizer + memory
5	Final integration, testing, presentation
