# 🧠 Clinical LLM Diagnostic Simulation – Demo (Thesis Project)

This demo showcases an agent-based diagnostic simulator using free, open-source LLMs via the OpenRouter API. The system evaluates diagnostic reasoning under biased patient behavior and generalizes to real-world cases extracted from the MIMIC-IV dataset.

---

## 📌 Project Features

- Simulates doctor-patient conversations using LLMs
- Supports 3 models: **Mistral**, **LLaMA**, **DeepSeek**
- Tests diagnostic accuracy under:
  - Normal interaction
  - Cancer-bias
  - Gender-bias
- Extends evaluation to **real clinical OSCE-style cases** (from MIMIC-IV)
- Outputs results as CSV files + accuracy graphs

---

## 🗂️ Project Structure

ClinicalLLM_Demo/
│
├── main.py # Runs all simulations and saves outputs
├── agents.py # Handles all LLM queries
├── dataset_loader.py # Loads MedQA and MIMIC-based cases
├── generated_mimic_osce.jsonl # Realistic clinical cases from MIMIC-IV
│
├── outputs/
│ ├── results_none_mistral.csv
│ ├── model_comparison_chart.png
│ └── ... more graphs & CSVs
│
├── .env # Contains your OpenRouter API key
├── requirements.txt # Required Python libraries
└── README.md # You are here

---

## 🔧 Setup Instructions

### 1. Clone the Repository or Download the Folder

```bash
git clone https://github.com/datascientistabhishek/Final_sem_thesis.git
cd Final_sem_thesis
###Create a .env File with Your API Key
OPENROUTER_API_KEY=sk-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
### Run the Simulation
python main.py

