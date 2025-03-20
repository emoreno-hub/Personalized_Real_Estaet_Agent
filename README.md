# Personalized Real Estate Agent

The goal of this project is to create a personalized experience for each buyer, making the property search process more engaging and tailored to individual preferences. This application leverages large language models (LLMs) and vector databases to transform standard real estate listings into personalized narratives that resonate with potential buyers' unique preferences and needs.

## Methodology
To achieve this, the project utilizes LangChain and ChromaDB:
- **LangChain:** LangChain provides a structured framework to interact with Large Language Models (LLMs). It simplifies prompt engineering, response parsing, and integration with external data sources, making it easier to generate high-quality real estate listings dynamically.

- **ChromaDB:** ChromaDB serves as a vector database to store and retrieve property listings based on semantic similarity. By converting property descriptions into vector embeddings, the system can quickly find and recommend relevant listings based on user queries, improving search accuracy beyond simple keyword matching.

## Core Components of "HomeMatch"

### Understanding Buyer Preferences

- Buyers will input their requirements and preferences, such as location, property type, budget, amenities, and lifestyle choices.
- The application uses **LLMs (powered by LangChain)** to interpret these inputs in natural language, understanding nuanced requests beyond basic filters.

### Integrating with a Vector Database

- "HomeMatch" connects with **ChromaDB**, a vector databases where all available property listings are stored.
- The system generates and stores vector embeddings for each listing, enabling semantic search that considers deeper aspects like neighborhood vibes, architectural styles, and proximity to specific amenities..

### Personalized Listing Description Generation

- For each matched listing, use an LLM to rewrite the description in a way that highlights aspects most relevant to the buyer’s preferences.
- Ensure personalization emphasizes characteristics appealing to the buyer without altering factual information about the property.

### Listing Presentation

- Output the personalized listing(s) as a text description of the listing.

## How to execute

1 - Clone this repository
```bash
https://github.com/emoreno-hub/Personalized_Real_Estaet_Agent.git
```

2 - Create the virtual environment

```bash
conda create --name agent --python==3.9.18
```

This step uses [Anaconda](https://www.anaconda.com/) as the environment manager, but feel free to use another one of your choice.

3 - Install the requirements

```bash
pip install -r requirements.txt
```


**Important**: You need to put your OpenAI key in the first cell to run the notebook.

```python
# Environment variables
OPENAI_API_KEY = 'YOUR API KEY'
```
It is highly recommended to use GPU to execute the code.
