# n8n AI workflow maker

[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/JAPozueloM.svg?style=social&label=Follow%20%40JAPozueloM)](https://twitter.com/JAPozueloM)

## What is this?
NOTE: This project is quite old and hasn't been updated since. It's still an interesting showcase of crude prompting techniques and vector DBs. If I were to re-do this project, I would probably generate a data set with whole n8n JSONs as answers to queries. If context is an issue then it might make sense to do 2 finetuned models. One for planning and one for the execution of each node. To create those data sets, you could go through the list of n8n nodes and generate usage examples for each. 


This is a tool where you input a natural language description of an automation workflow and it generates the workflow on n8n (Generates a JSON representation that you can copy and paste into the canvas)

The purpose of this project was to create an educational example of how to create complex GPT workflows which outputs are deterministic. Hopefully the n8n community and automation community in general will get more involved in AI and some collaboration can be achieved.

## Project parts

### Main n8n workflow
https://github.com/josepozuelo/n8nAIworkflow/tree/main/n8n_AI_workflows

### Embedding Store Creation REPL
https://replit.com/@JosePozuelo/GPT3embeddingstocsv#create_embeddings.py

### Pinecone vector store
https://app.pinecone.io/

### N8n node-list JSON

### If node parameters workflow
https://github.com/josepozuelo/n8nAIworkflow/tree/main/n8n_AI_workflows

### Resource/operation parameters workflow
https://github.com/josepozuelo/n8nAIworkflow/tree/main/n8n_AI_workflows

## How to use/explore?

Open the main JSON, it includes a walkthrough of the different stages. You can checkout the main prompt structures there as well as the main logic to create the n8n JSON for each generation.

Steps before running the workflow:
1. Create Pinecone account and get API keys (free)
2. Run the Embedding Store Creation REPL in your own Pinecone account
3. Create a Firestore account
4. Edit the three workflows in n8n_data_workflows to use the node-list and generate the parameter DB in your firestore instance

To visualize the workflow:
Just copy and paste each the whole contents of the JSON file into the n8n workflow editor. (https://app.n8n.cloud/dashboard)

After that you can explore the rest of the files included. If more people show interest I will document their usage better!
