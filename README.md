Automated Data Extraction and Classification with Machine Learning and OpenAI API

This project automates data extraction, classification, and tagging using machine learning models and the OpenAI API. It streamlines data ingestion from multiple file formats (XLSX, PDF, DOCX, TXT) and improves processing efficiency by 40%. With a robust ETL pipeline and advanced prompt generation, the system ensures accurate and consistent report classification.

Key Features

- Automated Data Extraction: Supports XLSX, PDF, DOCX, and TXT files.
- ETL Pipelines: Extracts, transforms, and loads data across datasets for reporting and analysis.
- Machine Learning Models: Achieves 91% accuracy in report classification, validated with performance metrics.
- OpenAI API Integration: Generates dynamic prompts to enhance classification and maintain consistency.

Installation
Prerequisites:

Python 3.8 or above
Install dependencies:
bash
Copy code
pip install pandas scikit-learn pdfplumber docx2txt openai
Set up OpenAI API:

python
Copy code
client = AzureOpenAI(
    azure_endpoint="<your-openai-endpoint>",
    api_key="<your-api-key>",
    api_version="2024-02-01"
)

Place Mapping Files: Ensure these files are in the project directory:

machine_mapping.csv
product_mapping.csv
report_mapping.csv
unit_mapping.csv

Usage
Run the Extraction and Classification Pipeline:

Use the notebook model.ipynb to extract and classify reports.

Example of file extraction:

python
Copy code
extracted_text, report_id = extract_text_from_file('sample_report.pdf')
print(extracted_text)
ETL Pipeline Execution:

python
Copy code
mapped_data = perform_etl_pipeline(input_data, machine_mapping, product_mapping)
print("ETL process completed!")
Save Mapped Data:

python
Copy code
df_mapped.to_csv('final_mapped_output.csv', index=False)
print("Mapped data saved to final_mapped_output.csv")
