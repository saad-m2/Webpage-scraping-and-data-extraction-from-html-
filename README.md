# Compliance Evidence Pipeline using LangGraph

A production-style AI pipeline that extracts structured company information from websites using LangGraph orchestration, Playwright for evidence collection, and Gemini API for LLM processing.

## How It Works

1. **Evidence Collection**: Playwright captures HTML content from websites
2. **AI Extraction**: Gemini API processes HTML to extract company information  
3. **Data Validation**: Pydantic validates extracted data with retry logic
4. **Report Generation**: Creates structured reports with findings
5. **Audit Logging**: Logs every step for compliance requirements

## Technology Stack

- **LangGraph**: Graph-based pipeline orchestration
- **Playwright**: Web automation and HTML capture
- **Gemini API**: AI-powered data extraction
- **Pydantic**: Data validation and schema enforcement
- **BeautifulSoup**: HTML preprocessing and cleaning

## Setup
```bash
pip install -r requirements.txt
playwright install
Run with: python main.py <url> 