# Structured Output Demo (LangChain + Pydantic + TypedDict + Google Gemini)

This repository demonstrates multiple ways to enforce structured outputs from LLMs (LangChain + Google Gemini or HuggingFace) using Python type‑safety tools (Pydantic models, JSON Schema, and TypedDict), plus a simple Pydantic data‑validation example.

---

## 📁 Repository Structure

| File | Description |
|-------|-------------|
| **pydantic_demo.py** | Shows basic Pydantic usage: defines a `Student` model, validates input data, and serializes to JSON. |
| **json_schema.json** | A standalone JSON Schema defining a minimal “student” object (title, type, required fields). |
| **structured_output_with_gemini.py** | Uses LangChain + HuggingFace endpoint to generate a review summary with a Pydantic schema for structured output. |
| **structured_output_with_json_schema.py** | Uses LangChain + Google Gemini with a raw JSON Schema to enforce output structure. |
| **typedict_test.py** | Demonstrates Python’s `TypedDict` for static‑type validated dictionaries. |
| **with_structured_output_pydantic.py** | Uses LangChain + Google Gemini with a Pydantic model to produce strongly typed review output. |
| **with_structured_output_typedict.py** | Uses LangChain + Google Gemini with a `TypedDict` schema for structured output and prints a specific field. |

---

## 🚀 Quick Start

1. Clone this repo  
   ```bash
   git clone https://github.com/<your-username>/structuredoutput.git
   cd structuredoutput
   ```

2. Create & activate a virtual environment  
   ```bash
   python3 -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate      # Windows
   ```

3. Install dependencies  
   ```bash
   pip install -r requirements.txt
   ```

4. Add your API key to a `.env` file  
   ```
   GOOGLE_API_KEY=your_gemini_api_key_here
   ```

5. Run any example script  
   ```bash
   python pydantic_demo.py
   python structured_output_with_gemini.py
   python with_structured_output_typedict.py
   ```

---

## 🔧 Tech Stack

- **LangChain** — orchestration  
- **Google Gemini (PaLM)** via `langchain-google-genai`  
- **Pydantic** & **TypedDict** — structured output schemas  
- **HuggingFaceEndpoint** — alternative LLM backend  
- **python-dotenv** — environment management  

---

## 📄 License

MIT © 2025

## 📫 Contact

Questions or feedback? Email **haseebulhassan1172003@gmail.com**.
