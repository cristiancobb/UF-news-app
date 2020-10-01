# UF-news-app

# Import 
import requests
import json
import pandas

# Filter 
url = ('http://newsapi.org/v2/top-headlines?'
       'q=country=us&'
       'from=2020-09-29&'
       'sortBy=popularity&'
       'apiKey=42d74772d5b849f4a7c3cfb0236c598e')

response = requests.get(url)

# Show top ten results
for i in range(10):
    googlenews.getpage(i)
    result=googlenews.result()
    df=pd.DataFrame(result)
list=[]

# List results
print response.json()
