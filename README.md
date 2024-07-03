# Assessment
This is the assessment prior to the interview.

Follow all the steps given in the in the assessment document. You are free to use any generative AI tools (ChatGPT, Claude, LLama etc.) for code generation/debugging. Make sure to include a comment for the part which was obtained using genAI tools.

#### Setup:
After the setup of Docker, ElasticSearch and Kibana given in the assessment document, we suggest setting up a new conda environment with elasticsearch7 python package and all the necessary packages installed (pandas, etc.)

#### Query/data processing instructions:
1. Use any text cleaning package to clean the data (from the .csv) before pushing the data to ElasticSearch.
2. Remove stopwords if you think its better.
3. Ideally write a python function to dio this and you are free to use the same function to process the queries from queries.txt.

#### Format of data to be pushed into ES index
You should convert each row of the ```assessment_data.csv``` file into the following format and push it to your ES index. 
```
{
    "id": 1,
    "title": "<data from the 'title' column of assessment_data.csv>",
    "tags": "<data from the 'tags' column of assessment_data.csv>",
    "url": "<data from the 'sourceURL' column of assessment_data.csv>",
    "category": "<data from the 'category' column of assessment_data.csv>"
}
```

Make sure you include instructions for running your code i.e., what command should be used to run your code. 

### NOTE: We require you to write all of your code as python scripts instead of Jupter notebook .ipynb files.
