# Cost-effective Dataset Creation, Model Fine-tuning and Vector Embeddings

This repository showcases a comprehensive methodology for generating versatile language datasets using LangChain and OpenAI. Further, it provides a guide to fine-tuning the Falcon-7b model to achieve refined performance using the generated dataset.
See the linkedin [post](https://www.linkedin.com/posts/kc-kosaraju_datascience-langchain-openai-activity-7094995764992479232-oK8q) for more details.

## Overview

In the evolving landscape of NLP, the diversity and quality of training datasets directly impact model performance. Our approach focuses on creating datasets enriched with various writing styles and then using this rich data to fine-tune sophisticated models like Falcon-7b.
## Dataset Generation

Utilizing the prowess of LangChain and OpenAI, we present a cost-effective and efficient approach to cultivate diverse datasets. Such a foundation is instrumental in encapsulating the full spectrum of human linguistic expression, fortifying the adaptability of ensuing models.

LangChain facilitates a seamless experience in crafting prompts for Language Learning Models (LLMs). While it's compatible with various models, our focus is on leveraging OpenAI's ChatGPT 3.5. The ambition is to architect a prompt adept at transmuting structured data into coherent, conversational prose.

Example:

Structured Data: 'Travelers: 5 persons, Travel Type: business, Meal Preference: fast food, Transportation: train, flight, Booking Mode: last minute deals, Cultural Interest: historical sites.'

Narrative:
"Planning a business venture for a quintet, our leanings are towards fast food and a mix of rail and air travel. We're scouting for eleventh-hour deals and are enthusiastic about immersing ourselves in historical locales."

## Fine-tuning Falcon-7b
Once the dataset is in place, we employ tools like transformers, bitsandbytes, and the accelerate libraries to enhance the Falcon-7b LLM. The fine-tuning is realized using the QLORA technique on our meticulously curated synthetic dataset.

## Vector Embeddings
With the assistance of LangChain and OpenAI, we generate vector embeddings to architect a Vector Database. We've integrated Facebook's FAISS to pinpoint similar queries and their associated responses, facilitating the transformation from unstructured to structured data.
