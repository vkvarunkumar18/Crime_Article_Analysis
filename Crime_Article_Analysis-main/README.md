# Crime Articles Analysis: Trends and Insights with Python

## Overview
This project analyzes a dataset of 7,617 unique crime articles (2005–2022) using Python to uncover temporal, categorical, and geographic trends in crime reporting. The analysis leverages data manipulation, visualization, natural language processing (NLP), and an interactive search interface to provide actionable insights into crime patterns. Key objectives include identifying peak crime reporting periods, dominant crime categories, and primary news sources, while enabling users to explore articles interactively.

## Dataset
The dataset contains 7,617 crime articles sourced primarily from `timesofindia.indiatimes.com`. It includes the following columns:
- **crime_articles**: `Heading`, `Content_summary`, `Article_link`, `Img_link`, `Month_date`, `Time`, `Year`

Derived columns created during analysis:
- `clean_year`: Extracted year for temporal analysis.
- `crime_category`: Categorized articles into types (e.g., Violent Crime, Financial Crime).
- `source`: Extracted news source for analysis.

## Project Structure
- **data/**: Contains `7K UNIQUE crime articles.csv`.
- **Analysis.ipynb**: Main notebook with the following sections:
  - **Data Preprocessing**: Loaded and cleaned data using pandas, extracted years, and categorized articles.
  - **Temporal Analysis**: Analyzed article distribution by year (2005–2022).
  - **Categorical Analysis**: Examined crime categories (e.g., Violent Crime, Arrests).
  - **Source Analysis**: Identified dominant news sources.
  - **Visualization**: Created bar charts using matplotlib/seaborn (e.g., articles by year).
  - **Interactive Interface**: Built a search tool with Jupyter widgets for filtering by keyword, category, and location.
  - **Geographic Analysis**: Laid groundwork for regional comparisons (e.g., Mumbai, Delhi).

## Key Findings
- **Temporal Trends**: Article volume grew significantly over time, peaking in 2021 (2,540 articles) and 2022 (2,216 articles), indicating increased crime reporting or media focus.
- **Crime Categories**: 
  - "Other" crimes were most frequent (4,406 articles), followed by Violent Crime (1,859) and Arrests (574).
  - Less frequent categories included Cyber Crime (91 articles) and Drug Crime (149 articles).
- **News Sources**: Over 96% of articles (7,381) were from `timesofindia.indiatimes.com`, with 236 from `m.timesofindia.com`.
- **Geographic Potential**: The dataset supports location-based analysis (e.g., Mumbai, Delhi), though further extraction of location data is needed for deeper insights.

## Technical Skills Demonstrated
- **Python Libraries**:
  - **pandas**: Data cleaning, manipulation, and analysis.
  - **matplotlib/seaborn**: Visualized trends with bar charts (e.g., articles by year).
  - **nltk/wordcloud**: Applied NLP for text preprocessing (tokenization, stopwords removal).
  - **ipywidgets**: Built an interactive search interface.
- **Data Analysis**: Performed temporal, categorical, and source-based analysis.
- **Visualization**: Created clear, insightful visualizations for trend identification.
- **Interactivity**: Developed a user-friendly interface for filtering articles by keyword, category, and location.
- **NLP Basics**: Processed article text for categorization and potential content similarity analysis.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/MalleshHV/Crime_Article_Analysis
2. Install dependencies:
   ```bash
    pip install pandas matplotlib seaborn nltk wordcloud ipywidgets
3. Download NLTK data:
   ```bash
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
4. Ensure the dataset (7K UNIQUE crime articles.csv) is in the data/ folder.
5. Launch the notebook:
   ```bash
   jupyter notebook SDP3.ipynb
6. Run all cells to reproduce the analysis and interact with the search interface.


## Future Improvements
 - **Geographic Analysis**: Extract and map locations (e.g., using regex or NLP) for regional comparisons.
- **Sentiment Analysis**: Analyze the tone of articles (positive, negative, neutral) using NLP.
- **Advanced NLP**: Implement topic modeling (e.g., LDA) to identify recurring themes in crime reporting.
- **Performance Optimization**: Use Dask or multiprocessing for faster processing of large text datasets.
- **Enhanced Interactivity**: Add date range filtering and visualization options (e.g., time series plots) to the search interface.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [YouTube Data API](https://developers.google.com/youtube/v3)
- [Pandas](https://pandas.pydata.org/), [Matplotlib](https://matplotlib.org/), [Seaborn](https://seaborn.pydata.org/) for data analysis and visualization.
- [NLTK](https://www.nltk.org/) for natural language processing.


## Contact

For any questions or feedback, please contact at vk.varunkumar1818@gmail.com.
