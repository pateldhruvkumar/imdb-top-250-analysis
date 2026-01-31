# IMDB Top 250 Movies Analysis

This project scrapes and analyzes the IMDB Top 250 movies chart to extract detailed information about the highest-rated films of all time. It utilizes Python with web scraping libraries to fetch, parse, and structure the data for analysis.

## 📋 Project Overview

The main objective of this project is to programmatically retrieve the current top 250 movies from IMDB and compile them into a structured dataset. 

**Key Features:**
- Fetches real-time data from IMDB.
- Uses robust JSON parsing (targeting `__NEXT_DATA__`) to extract reliable data even if the UI layout changes.
- Extracts comprehensive movie details including metadata not always visible on the main list.

## 🛠️ Technologies Used

- **Python**: Primary programming language.
- **Requests**: For making HTTP requests to fetch the webpage.
- **BeautifulSoup (bs4)**: For parsing HTML content.
- **Pandas**: For data manipulation and exporting to CSV/Excel.
- **JSON**: For parsing the embedded data structures within the webpage.

## 📊 Data Extracted

For each movie in the Top 250, the following information is extracted:
- **Rank**: Position in the Top 250 chart.
- **Title**: Movie title.
- **Year**: Release year.
- **Rating**: IMDB aggregate rating (e.g., 9.3).
- **Rating Count**: Number of user votes.
- **Duration**: Runtime in hours and minutes (and raw seconds).
- **Genre**: List of genres associated with the movie.
- **Content Rating**: Certificate/Age rating (e.g., R, PG-13).
- **IMDB ID**: Unique identifier for the movie on IMDB.
- **URL**: Direct link to the movie's IMDB page.

## 🚀 Getting Started

### Prerequisites
Ensure you have Python installed. You can verify this by running:
```bash
python --version
```

### Installation
Install the required Python libraries using pip:

```bash
pip install requests beautifulsoup4 pandas
```

### Running the Analysis
1. Open the notebook file `EAI6000_Dhruvkumar_Task2.ipynb` in Jupyter Notebook, JupyterLab, or VS Code/Cursor.
2. Run the cells sequentially to:
   - Import libraries.
   - Configure the scraper.
   - Fetch the IMDB page.
   - Parse the JSON data.
   - Verify and display the results.

## 📝 Methodology

Instead of relying solely on HTML class names which can change frequently, this scraper targets the `__NEXT_DATA__` JSON blob embedded in the IMDB page source. This approach is more stable and allows for extracting richer data attributes that are passed to the frontend framework.

## 👤 Author

**Dhruvkumar**  
Course/Task: EAI6000 - Task 2
