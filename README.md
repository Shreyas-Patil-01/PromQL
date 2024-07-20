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


## Project Overview

### Description
This project provides a powerful tool for translating natural language queries into PromQL (Prometheus Query Language) using a fine-tuned machine learning model. By leveraging the Gemini version 1 model on Vertex AI, this project aims to bridge the gap between human-friendly query expressions and the complex syntax of PromQL.

### Objectives
- **Simplify Query Creation**: Enable users to write queries in plain English, eliminating the need to learn PromQL syntax.
- **Enhance Accessibility**: Make querying Prometheus metrics more accessible to users who may not be familiar with PromQL.
- **Increase Productivity**: Speed up the process of generating and modifying PromQL queries, particularly useful for those who frequently work with time-series data.

### Features
- **Natural Language Input**: Users can input their queries in natural language.
- **Accurate Translation**: The model translates natural language queries into precise PromQL queries.
- **Customizable**: Fine-tuned on a custom dataset to handle specific types of queries relevant to your use case.
- **User-Friendly**: Easy-to-use interface that simplifies the process of querying Prometheus.

### Benefits
- **User-Friendly Interface**: No need to learn complex query languages—just describe what you need in plain language.
- **Improved Efficiency**: Quickly generate PromQL queries without manually writing them, reducing time spent on query development.
- **Flexibility**: Adaptable to various use cases by fine-tuning the model on different datasets.

### Workflow
1. **Input Query**: Enter a natural language description of the query you want.
2. **Model Processing**: The fine-tuned model processes the input and converts it into a PromQL query.
3. **Output**: Receive the generated PromQL query that you can use directly in Prometheus.

### Visual Representation
![Project Workflow](https://github.com/Shreyas-Patil-01/PromQL/blob/main/model_deployed_img.png)
![Project Workflow](https://github.com/Shreyas-Patil-01/PromQL/blob/main/Fine_tuned_model_details.png)
![Project Workflow](https://github.com/Shreyas-Patil-01/PromQL/blob/main/output_video.mp4)

This diagram illustrates the end-to-end process of converting a natural language query into PromQL using the fine-tuned model.

### Examples
- **Performance Monitoring**: Translate queries related to server performance into PromQL to monitor metrics.
- **Alerting**: Generate PromQL queries to set up alerts based on specific conditions described in natural language.
- **Reporting**: Convert user-friendly queries into PromQL for generating reports on system metrics.

By providing a straightforward way to translate natural language into PromQL, this project makes querying Prometheus metrics more accessible and efficient for users of all skill levels.


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
5. Access through its endpoint by requesting the model.

### Installation
Clone this repository and install the required dependencies:
```bash
git clone https://github.com/Shreyas-Patil-01/PromQL.git
cd PromQL

