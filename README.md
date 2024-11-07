# spatiAlytica: a large language model for analyzing HTAN spatial transcriptomics data 

## Team members
Team Leader: Arun Das

Tech Lead: Krithika Bhuvaneshwar

Writers: Jeanna Arbesfeld-Qiu, Sanna Madan, Noam Gaiger

Members: Ashish Mahabal, Khoa Huynh, Mingyu Yang, Noam Gaiger

## Background
*In situ* spatial transcriptomic (ST) technologies are a breakthrough class of methods that have redefined cancer biology research by providing insight into tumor microenvironment structure, organization, and heterogeneity. ST data have also allowed researchers to understand cell-cell signaling, such as in the context of the tumor microenvironment or the formation of developmental gradients. 

## What's the problem?
A growing number of spatial databases are being generated and are publicly available, yet navigating them can be challenging. For example, the Human Tumor Atlas Network (HTAN) is a valuable resource for biomedical researchers; however, making the data more easily accessible will potentiate its effective use. The large-scale and complex data generated by ST requires the development of specific tools for data analysis and interpretability. Currently, such tools require the computational expertise of a trained bioinformatician and close collaboration between wet-lab and dry-lab scientists.

## Our solution: spatiAlytica

SpatiAlytica is a multiagent large language model specifically designed to analyze spatial transcriptomic data from the Human Tumor Atlas Network (HTAN). SpatiAlytica allows users to interact with datasets on HTAN using conversational, natural language queries, making spatial transcriptomics analysis accessible to those with limited expertise in bioinformatics.

## Approach
Our approach uses three agents to allow for:
- Data integration with HTAN resources
- Bioinformatics analysis using standard Python packages
- Interactive chat interface providing human-friendly output

A reasoning engine directs the user's queries to the correct agent.
<div style="text-align: center;">
  <img width="617" alt="image" src="https://github.com/user-attachments/assets/dc634dd7-6013-4b68-94c8-089ca1396378">
  <img width="546" alt="image" src="https://github.com/user-attachments/assets/6665cbd9-34cb-49fb-9d17-95cf8710c8a8">
</div>

## Examples of questions you can ask spatiAlytica:
* Download all datasets in HTAN with 10x Visium spatial information for melanoma.
* What is the expression level of gene x in sample y?
* Show me the spatial location of the malignant cells.

## Our workflow details
<img width="619" alt="Screenshot 2024-11-07 at 8 58 26 AM" src="https://github.com/user-attachments/assets/9bff23be-f4e4-4587-8d51-a074d3fa2598">

## Installation

### Platform Requirements
spatiAlytica is designed to run on Google Cloud Platform's Vertex AI.

### Dependencies
Required Python packages:
```python
synapseclient==4.6.0
scanpy==1.10.3
squidpy==1.6.1
pandas==2.2.2
matplotlib==3.7.1
google==2.0.3
vertexai==1.70.0
anndata-0.11.0



