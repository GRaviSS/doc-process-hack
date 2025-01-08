# Challenge 3 - Data Modelling: From Retrieval to Upload

**Expected Duration:** 60 minutes

## Introduction
Your goal in this challenge is to get introduced to the concept of integrating Azure AI Document Intelligence API, retrieving custom data to enhance several business processes. 
You will learn how to handle different data structures and upload and manage text content in a Cosmos DB container. 
Additionally, you will explore how to efficiently store and retrieve data, enabling streamlined workflows and effective data management.

## Our Scenario

As per the nature of our workshop, now we have to *divide and conquer*. We have now saved the `.json`files of our 3 types of documents, but the way to process each one of the documents is intimately related with their structure. As so, we
we will divide our workshop into 3 Guides. Each one of the Guides is therefore divided into 2 main parts:
- **Data Modelling:** It's time to structure how JSON file, modelling and retrieving the information we need. Some of the data will be structured into tables, while some other data will be formatted as text. This step ensures that the extracted information is organized in a meaningful way for further analysis and usage.
- **Data Upload:** Now that we have created the JSON structure desidered, we  will upload it into our Azure Cosmos DB container.
- **Data Cleaning:** On Guide number 3 you will have your first code-first challenge.

## Guide 1 : Extract Information from Loan Forms

Please jump over to the `loanforms_modelling.ipynb` file to complete this guide.

## Guide 2 : Extract Information from Pay Stubs 

Please jump over to the `paystub_modelling.ipynb` file to complete this guide.

## Guide 3 : Extract Information from Loan Agreements

Please jump over to the `loanagreements_modelling.ipynb` file to complete this guide.

## Upload the Terms and Conditions of House Loans  (optional)

Great! We have now created some functions made to process very **specific** documents. As you might realise, these are not generic, and for good reason: we want to ensure that in the end of our solution, we have a well (semi-)strutured DB with this information. However, as you might know, some documents are a bit more generic.

In the future our company will think about creating a chatbot that will integrate bank's documents and customer information. As so, you can find on this Challenge also a `houseloan.pdf`file, that you can also upload to your Storage Account, OCR the document using Document Intelligence and clean the data s much as possible.

**NOTE:** This challenge is optional. If you want to learn more about using the Document Intelligence client API follow the [documentation]([https://docs.microsoft.com/en-us/azure/storage/blobs/storage-quickstart-blobs-python](https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/how-to-guides/use-sdk-rest-api?view=doc-intel-4.0.0&tabs=windows&pivots=programming-language-python)) and create a **new notebook** that will process the T&C for House Loans.

## Conclusion
In this challenge, you learned how to clean and prepare text data for uploading to Azure Cosmos DB. You utilized Python to handle and process text content, ensuring it is properly formatted and free of errors before storage. You created functions to check for empty text content, initialize the Cosmos client, and manage databases and containers. Additionally, you learned how to handle potential errors during the upload process. The concepts learned in this challenge are applicable to other scenarios where data cleaning and preparation are required, enabling you to automate and streamline data management workflows.
