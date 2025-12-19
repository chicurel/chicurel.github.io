---
title: 'Electoral Programs OCR Pipeline'
summary: 'AI-based OCR and multilingual processing pipeline for historical electoral manifestos, including sentence-level extraction and translation'
authors:
  - 2025
date: '2025-01-01T00:00:00Z'

tags:
  - AI
  - Data Analysis
  - LLMs
  - Machine Learning
  - Python


url_project: 'https://github.com/chicurel/electoral-programs-ocr-pipeline'
url_code: 'https://github.com/chicurel/electoral-programs-ocr-pipeline/blob/main/individual_files.ipynb'
url_pdf: ''
url_dataset: ''
url_slides: ''
url_video: ''

---

# Electoral Manifestos OCR Pipeline

This repository contains the **core Python workflow** ("código madre") for processing historical electoral programs using **AI-based OCR**, sentence-level text segmentation, and **automatic translation** into Spanish or English.

The pipeline is designed to be **reproducible, scalable, and user-friendly**, so that research assistants without deep text-as-data expertise can process new electoral programs as they are incorporated into the project.

---

## Project Overview

The workflow follows these steps:

1. **AI-based OCR of PDF files**
   Electoral programs in PDF format are processed using **Mistral OCR**, which extracts high-quality text from scanned or native PDFs.

2. **Sentence-level segmentation**
   Extracted text is split into individual sentences, with **one sentence per row**, enabling downstream text-as-data analysis.

3. **Language detection and translation**
   Sentences not written in Spanish or English (e.g. French) are automatically translated **sentence by sentence** using **ChatGPT**.

4. **Structured output**
   The results are stored in structured formats (Markdown and DataFrames) that can later be used for:

   * Manual or automated coding
   * Machine learning classification (e.g. CAP / Babel models)
   * Comparative political text analysis

---

## Input Data

* **Format:** PDF files
* **Typical content:** Historical electoral programs / manifestos
* **Naming convention:**

  ```
  region_year_party_language.pdf
  ```

  Example:

  ```
  quebec_1994_pq_fr.pdf
  ```

This naming system is important for tracking documents consistently across the project.

---

## Output

For each PDF, the pipeline generates:

* A **Markdown (.md) file** containing the extracted OCR text
* A **DataFrame** with:

  * Document identifier (filename)
  * Full extracted text
  * Sentence-level representations (after segmentation)
  * Translated sentences when applicable

Each sentence occupies **one row**, making the output ready for coding and analysis.

---

## Requirements

Main Python dependencies:

* `python >= 3.9`
* `pandas`
* `numpy`
* `spacy`
* `mistralai`
* `openai`

You will also need:

* **Mistral API key** (for OCR)
* **OpenAI API key** (for translation)

Make sure your API keys are available as environment variables, for example:

```bash
export MISTRAL_API_KEY="your_key_here"
export OPENAI_API_KEY="your_key_here"
```

---

## How to Use

1. Place PDF files in the designated input folder.
2. Open and run the notebook `individual_files.ipynb`.
3. The script will:

   * Send PDFs to Mistral OCR
   * Extract and clean the text
   * Split text into sentences
   * Translate non-English/Spanish content
   * Save outputs automatically

The notebook is intentionally written in a **step-by-step and readable way** to facilitate use by non-expert research assistants.

---

## Future Extensions

This repository is intended as a foundation for:

* Automated coding using CAP / Babel models
* ChatGPT-based supervised classification
* Cross-national and longitudinal manifesto analysis
