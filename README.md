## Youtube-Search-Bot-Python
A python library that uses browser automation to search keyword on youtube and fetch search results automatically.
At present, it runs on Windows only.
It uses [datakund](https://pypi.org/project/datakund) internally

Complete Documentation available [here](https://youtube-api.datakund.com/en/latest/)


### Support
For any help / feedback you can message us here
* datakund@gmail.com
* https://t.me/datakund

### Installation

```sh
pip install youtube-auto-search
```

### Import

```javascript
from youtube-auto-search import *
```

### Search Keyword

To search keyword on youtube we use ``search`` function
It requires **keyword** as input parameter

```javascript
youtube.search(keyword="search_term_here")
```

### Fetch Search Results

To fetch search results we use ``search_results`` function.
It does not require any input parameter.
It tries to fetch youtube search results of whichever page is opened

```javascript
response=youtube.search_results()
results=response['body']
```

### Example Response

```sh
[
   {
      "viewsandtime":"viewsandtime",
      "channel":"channel",
      "title":"title",
      "link":"link"
   },
   {
      
   },
   "..."
]
```

### DataKund
It uses [datakund](https://pypi.org/project/datakund/) internally to do browser automation
DataKund is an automation library that uses selenium & supports automation of many sites including [Youtube](https://youtube-api.datakund.com/en/latest/), [Amazon](https://amazon-api.datakund.com/en/latest/), [Twitter](https://twitter-api.datakund.com/en/latest/), [LinkedIn](https://linkedin-api.datakund.com/en/latest/) , [Google](https://google-api.datakund.com/en/latest/) etc.
