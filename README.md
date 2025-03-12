# Mars News and Weather Data Scraping Project

## Project Overview
This project involves web scraping and data analysis of Mars-related information. It is divided into two main deliverables:

1. **Scraping Mars News Articles** – Extracting titles and preview text from a Mars news website.
2. **Scraping and Analyzing Mars Weather Data** – Extracting weather data from an HTML table and performing an analysis.

## Technologies Used
- Python
- Jupyter Notebook
- Beautiful Soup
- Pandas
- Matplotlib

## Deliverables

### Deliverable 1: Scrape Titles and Preview Text from Mars News

#### Steps:
1. **Automated Browsing** – Visit the Mars news website ([Mars News](https://static.bc-edx.com/data/web/mars_news/index.html)) using a web scraping script.
2. **Inspect & Extract Data** – Identify the necessary HTML elements and extract the article titles and preview text using Beautiful Soup.
3. **Store Data** – Save the extracted information in a Python dictionary, where each dictionary entry contains:
   ```python
   {
       "title": "Article Title",
       "preview": "Article Preview Text"
   }
   ```
4. **List of Dictionaries** – Store all extracted articles in a list.

### Deliverable 2: Scrape and Analyze Mars Weather Data

#### Steps:
1. **Automated Browsing** – Access the Mars Temperature Data website ([Mars Temperature Data](https://static.bc-edx.com/data/web/mars_facts/temperature.html)).
2. **Extract Data** – Scrape the HTML table using Beautiful Soup.
3. **Data Cleaning** – Convert the extracted data into a Pandas DataFrame with the following columns:
   - `id`: Identification number of a single transmission from Curiosity.
   - `terrestrial_date`: Date on Earth.
   - `sol`: Number of elapsed Martian days (sols) since Curiosity landed.
   - `ls`: Solar longitude.
   - `month`: Martian month.
   - `min_temp`: Minimum temperature (°C) for a Martian day.
   - `pressure`: Atmospheric pressure at Curiosity’s location.
4. **Data Type Conversion** – Ensure appropriate data types (datetime, int, float) are used.
5. **Analysis & Insights:**
   - Determine the number of Martian months.
   - Count the total number of Martian days recorded.
   - Identify the coldest and warmest months by computing average minimum temperatures and visualize using a bar chart.
   - Identify the months with the lowest and highest atmospheric pressure, then visualize using a bar chart.
   - Estimate the length of a Martian year by plotting daily minimum temperatures over time.
6. **Export Data** – Save the cleaned DataFrame as a CSV file for further analysis.

## How to Run the Project
1. Clone the repository or download the project files.
2. Install dependencies using:
   ```bash
   pip install beautifulsoup4 pandas matplotlib
   ```
3. Open the Jupyter Notebooks:
   - `part_1_mars_news.ipynb` for scraping news articles.
   - `part_2_mars_weather.ipynb` for scraping and analyzing Mars weather data.
4. Run each cell step-by-step to execute the web scraping and analysis.

## Results and Insights
- Extracted Mars news titles and previews.
- Collected and structured weather data from Mars.
- Identified temperature trends and atmospheric pressure variations across Martian months.
- Estimated the number of Earth days in a Martian year using temperature analysis.

## References
- Mars News Website: [https://static.bc-edx.com/data/web/mars_news/index.html](https://static.bc-edx.com/data/web/mars_news/index.html)
- Mars Temperature Data: [https://static.bc-edx.com/data/web/mars_facts/temperature.html](https://static.bc-edx.com/data/web/mars_facts/temperature.html)

## License
This project is for educational purposes and follows an open-source license.



