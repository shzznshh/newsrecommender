# Project Title
## News Recommender
# Project Description
## What it does?
##### A news recommendation system is an application that recommends news article 
based on the news a user is already reading using python.
## How does it work?
##### 
- When visiting News Portal site, on its landing page you’ll stumbled upon a recommendation section where it recommends similar content based on what you are already watching or reading
- Most popular news portal site uses content based recommendation systems specifically designed to find similarities between the news articles that you are already read on their site or other news portal site to recommend similar articles
- The dataset that was used in this project is from [newsapi.org](http://newsapi.org) where you would have to sign up in order to retrieve an api key. For this project, we’re using top headlines in the U.S.
- Here we will be uploading the following packages in order to retrieve data from newsapi site
    
    ```python
    # Upload packages
    import requests
    import pandas as pd
    import os
    
    # Read JSON objects
    key = "3026e0d9c0c94df2ac184e6b103d28c7"
    usnewsapi = requests.get("https://newsapi.org/v2/top-headlines?country=gb&apiKey=3026e0d9c0c94df2ac184e6b103d28c7").json()
    ```
    
- In this project, we will be using the news articles as the feature to find similar articles. A more accurate recommendation system for news.
