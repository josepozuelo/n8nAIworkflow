# n8n AI workflow maker

[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/JAPozueloM.svg?style=social&label=Follow%20%40JAPozueloM)](https://twitter.com/JAPozueloM)

## What is this?

This is a tool where you input a natural language description of an automation workflow and it generates the workflow on n8n (Generates a JSON representation that you can copy and paste into the canvas)
You can try it out here: https://tally.so/r/wM1bl0

The purpose of this project was to create an educational example of how to create complex GPT workflows which outputs are deterministic. Hopefully the n8n community and automation community in general will get more involved in AI and some collaboration can be achieved.

## Project parts

### Main n8n workflow

### Embedding Store Creation REPL
https://replit.com/@JosePozuelo/GPT3embeddingstocsv#create_embeddings.py

### Pinecone vector store


### N8n node-list JSON

### If node parameters workflow

### Resource/operation parameters workflow

## How to use/explore?

Open the main JSON, it includes a walkthrough of the different stages. You can checkout the main prompt structures there as well as the main logic to create the n8n JSON for each generation.

In order to run the main workflow, you first have to run the Embedding Store Creation REPL in your own Pinecone account (free). You also have to create a firebase DB with the operation/resource pairs for the Resource/operation parameters workflow

After that you can explore the rest of the files included. If more people show interest I will document their usage better!
