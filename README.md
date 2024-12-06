# webscraping-challenge
This challenge was broken down into two parts: Part 1-Scrape Titles and Preview Text from
Mars News, and Part 2-Scrape and Analyze Mars Weather Data.

Part 1: Scrape Titles and Preview Text from Mars News

Using automated browsing with Splinter and BeautifulSoup, a Google Chrome page
https://static.bc-edx.com/data/web/mars_news/index.html was visited. After inspecting the page
and its structure, BeautifulSoup was used to parse the HTML content and locate the elements
containing article titles and preview texts ('div' with class 'list_text'). For each article,
the title and preview were extracted and stored in a dictionary with keys 'title' and 'preview'.
The dictionaries were then appended to a Python list, and the list was printed in the provided
Jupyter Notebook. Once finished the browser session was closed. 

Part 2: Scrape and Analyze Mars Weather Data

Using Splinter and BeautifulSoup again, a table containing Mars weather data was scraped from
a webpage. The scraped data was then organized into a Pandas DataFrame. The columns were given
the same headings as the table on the website. The dataset was analyzed to answer the following
questions: "How many months exist on Mars", "How many Martian days worth of data exist in the 
scraped dataset?", "What are the coldest and warmest months on Mars(at the location of Curiousity)",
"Which months have the lowest and the highest atmospheric pressure on Mars?", "About how many
terrestrial (Earth) days exist in a Martian year?". After some data manipulation and analysis 
conducted, its concluded that: Mars has 12 months, there are 1867 'sols' or Martian days worth 
of data in the dataset, Month 3 has the lowest temperature on average while Month 8 has the highest,
Month 6 has the lowest atmospheric pressure while Month 9 has the highest on average, and there
are approximately 650 Earth days in a Martian Year. 
The cleaned data was saved to a provided CSV file. Finally the browser was closed.
