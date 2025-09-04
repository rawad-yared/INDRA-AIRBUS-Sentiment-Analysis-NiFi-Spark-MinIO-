# INDRA-AIRBUS-Sentiment-Analysis-NiFi-Spark-MinIO-
This was a modern data architecture project I worked on in my first term. The aim was to use a market stack API to collect stock prices of INDRA and AIRBUS through NiFi, store in MinIO, then use a spark session on jupyter notebooks to analyze and run a sentiment analysis from news sources 

File 1: 250722_Executive Presentation_Ed.F
- This file describes our findings and presentation that summarized the outcome of the project

File 2: G4_Ingestion_AIRBUS_+_INDRA
- This is the NiFi flow that can be imported and used to ingest the stock price data
- Note: The api within the flow is referencing my current market stack account which needs to be updated for personal use
- Note2: Make sure MinIO is enabled and that the bucket name matches the one in the put processor within the flow to ensure proper storage
- Note3: This flow has controller processes which need to be enabled

File 3: group_4_MDABD.ipynb
- This file is the jupyter notebook where all our code to initiate the spark session and run the data analysis was used
- Please note that Vader was used for sentiment analysis and that has to be configured in the terminal prior to running

File 4: news_indra_airbus_nato_last...
- This is a file with all the news headlines related to indra, airbus, or nato that was used in our sentiment analysis
