# Web Scraping using Beautiful Soup

The rt_html folder contains the Rotten Tomatoes HTML for each of the Top 100 Movies of All Time. https://www.rottentomatoes.com/


I'm saving these historical files because the ratings will change over time and there will be inconsistencies Also, a web page's HTML is known to change over time. Scraping code can break easily when web redesigns occur, which makes scraping brittle and not recommended for projects with longevity. 

## Beautiful Soup

Beautiful Soup parses anything you give it, and does the tree traversal stuff for you. You can tell it "Find all the links",
or "Find all the links of class externalLink", or "Find all the links whose urls match "foo.com", or "Find the table heading that's got
bold text, then give me that text."

So I'm using Beautiful Soup to extract our desired Audience Score metric and number of audience ratings,
along with the movie title for each HTML file, then save them in a pandas DataFrame.

For more information about Beautiful Soup check out the following documentation: 
- https://www.crummy.com/software/BeautifulSoup/
- And this article about Ethics in Web Scraping
  - https://towardsdatascience.com/ethics-in-web-scraping-b96b18136f01

