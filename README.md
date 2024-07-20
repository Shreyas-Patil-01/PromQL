# PromQL

# Natural Language to PromQL Translator

This repository contains the code and resources for a machine learning model that translates natural language queries into PromQL (Prometheus Query Language). The model is fine-tuned on Vertex AI using the Gemini version 1 base model.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Fine-Tuning](#model-fine-tuning)
- [Usage](#usage)
- [Installation](#installation)
- [Examples](#examples)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
This project aims to simplify the creation of PromQL queries by allowing users to input their queries in natural language. The fine-tuned model interprets the input and generates the corresponding PromQL query.

## Dataset
The dataset used for fine-tuning contains over 500 rows, each with two columns:
- `instruction`: Natural language prompts
- `output`: Corresponding Prometheus queries

The dataset is sourced from Hugging Face and has been customized for this project.

## Model Fine-Tuning
The model was fine-tuned using Vertex AI. The steps involved in the fine-tuning process include:
1. Preparing the dataset
2. Configuring the Vertex AI environment
3. Fine-tuning the Gemini version 1 model
4. Evaluating the model's performance

## Usage
To use this model, follow the steps below:
1. Install the necessary dependencies.
2. Load the fine-tuned model.
3. Input a natural language query.
4. Receive the corresponding PromQL query as output.

### Installation
Clone this repository and install the required dependencies:
```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
