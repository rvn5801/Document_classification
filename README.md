# Automated Document Classification using Hierarchical Taxonomy with LLMs

This repository contains the final project report and implementation details for **Group 25**, titled **"Automated Document Classification using Hierarchical Taxonomy with LLMs"**. The project focuses on leveraging **Large Language Models (LLMs)** to automate taxonomy enrichment and document classification with minimal supervision.

---

## **Project Overview**

The goal of this project is to develop a semi-automated system for **taxonomy enrichment** and **document classification** using advanced machine learning techniques. By leveraging LLMs, the system achieves high accuracy and scalability while minimizing the need for labeled data.

### **Key Features**
- **Taxonomy Enrichment**: Automates the process of enriching existing taxonomies using LLMs.
- **Document Classification**: Classifies documents with high accuracy using state-of-the-art models.
- **Minimal Supervision**: Reduces dependency on labeled data through semi-supervised learning.
- **Scalable Architecture**: Built on **AWS services** (S3, Lambda, OpenSearch) for real-time processing and retrieval.

---

## **Methodology**

The system employs a modular pipeline consisting of the following steps:

1. **Document Preprocessing**:
   - Text cleaning, stopword removal, and tokenization.
2. **Core Class Annotation**:
   - Uses **roberta-large-mnli** for initial document classification.
3. **Taxonomy Enrichment**:
   - Leverages **bert-base-uncased** and **all-MiniLM-L6-v2** for semantic similarity analysis.
4. **Text Classification**:
   - Utilizes **BiLSTM** and **sentence-transformers** for accurate document classification.
5. **Integration with AWS**:
   - Stores predictions in **Amazon S3**, triggers **AWS Lambda** for processing, and indexes data in **OpenSearch** for fast retrieval.

---

## **Results**

The system demonstrated significant improvements in taxonomy enrichment and classification accuracy:

- **Accuracy**: Achieved over **73%** in multiple datasets.
- **Precision-Recall Scores**: Robust identification and classification of entities.
- **Scalability**: Successfully adapted to diverse domains with minimal adjustments.

### **Example Use Case**
The system was tested on **Amazon Fashion Products**, where it accurately classified products into categories such as **Sandals**, **Flip-Flops**, and **Heeled Sandals**.

---

## **Future Work**

1. **Exploring New Methodologies**:
   - Incorporate unsupervised learning for improved generalization.
2. **Addressing Scalability**:
   - Optimize computational efficiency for larger datasets and real-time processing.
3. **Expanding Applicability**:
   - Adapt the solution for industries like healthcare, finance, and legal sectors.
4. **Multilingual and Multicultural Validation**:
   - Conduct case studies in diverse settings to ensure robustness.

---

## **Contributors**

- **Badrinath Reddy Panyam**: Backend development, UI design, OpenSearch integration.
- **Venkata Narayana Redrouthu**: ETL pipeline design, model evaluation.
- **Manoj Praveen Nandigama**: Data preprocessing, ML model implementation, OpenSearch setup.
