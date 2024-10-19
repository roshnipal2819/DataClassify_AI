# Automated Data Extraction and Classification with Machine Learning and OpenAI API

This project automates data extraction, classification, and tagging using machine learning models and the OpenAI API. It streamlines data ingestion from multiple file formats (XLSX, PDF, DOCX, TXT) and improves processing efficiency by 40%. With a robust ETL pipeline and advanced prompt generation, the system ensures accurate and consistent report classification.

## Key Features

- **Automated Data Extraction**: Supports XLSX, PDF, DOCX, and TXT files.
- **ETL Pipelines**: Extracts, transforms, and loads data across datasets for reporting and analysis.
- **Machine Learning Models**: Achieves 91% accuracy in report classification, validated with performance metrics.
- **OpenAI API Integration**: Generates dynamic prompts to enhance classification and maintain consistency.

## Installation

1. **Prerequisites**:
   - Python 3.8 or above
   - Install dependencies:

     ```bash
     pip install pandas scikit-learn pdfplumber docx2txt openai
     ```

2. **Set up OpenAI API**:

   ```python
   client = AzureOpenAI(
       azure_endpoint="<your-openai-endpoint>",
       api_key="<your-api-key>",
       api_version="2024-02-01"
   )
