
# :zap: Web scrapping using python, beautiful soup and pandas

This Python project makes use of web scraping techniques with Requests library and Beautiful Soup to extract movie details from The Movie Database (TMDb) and organizes the data using the Pandas library. The goal is to scrape information about movies from the TMDb website and transfer the data of first 50 pages into excel.


## Tools and Technologies Used

**Python:** The primary programming language for this project.

**Requests:** A Python library for making HTTP requests. It's used to fetch the HTML content of TMDb pages.

**Beautiful Soup:** A Python library imported from bs4 for pulling data out of HTML and XML files. It's used for web scraping in this project.

**Pandas:** A powerful data manipulation library for Python. It's used to handle and structure the scraped data.

**Excel:** The data is exported to an Excel spreadsheet for easy analysis and sharing.
## Project Workflow

1. **Basic setup:**
   - First import the requests and Beautiful Soup libraries.
   - Store the url of TMDb in a variable and use a header to prevent getting blocked trying to make multiple requests to the site.
   - Now create a function called get_all_pages() to generate the list of url of 50 pages using a for loop for web scraping.

2. **Web Scraping with Beautiful Soup and Requests:**
   - First iterate the list of 50 pages.
   - Within each page use a function called get_movie_cards() using requests library to fetch the HTML content of each movie from TMDb and using Beautiful Soup library parse the HTML and extract movie card detail.
   - iterate movie cards for each page and use fetch_movie_urls() function to generate a link to individual movie page.
   - Then use the requests and Beautiful Soup libraries to get the movie details in each page such as movie name, release date, rating, duration, director and genre while using fuctions to fetch each detail stored in respective variables.
   - Store all movie details in a dictionary called movie_dict and then append to a list called final_data.

3. **Data Structuring with Pandas:**
   - Use a function called save_to_excel(final_data) to create a Pandas DataFrame as df to organize the extracted data.
   - Clean and preprocess the data as needed (handling missing values, converting data types, etc.).
   - Using the to_excel() of DataFrame export the data as an excel file.
## Screenshots

![Exported Data in Excel](https://github.com/Dewang06/Web-Scrapping-Project/blob/main/themoviedb_excel.JPG)


## Authors

- [@Dewang06](https://github.com/Dewang06/Web-Scrapping-Project)


## About me

Hello everyone! I'm Dewang a recent graduate in BE Computer and an aspiring data analyst, to embark on an exciting journey in the world of data. I am thrilled to dive into the dynamic realm of the data. I eagerly embrace the opportunities to broaden my knowledge and skills.

I'm actively seeking opportunities to refine my skills. I'm committed to honing my skills in data analysis and ML.
