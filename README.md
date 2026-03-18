# Netflix Data Analysis

## Project Overview

This project performs exploratory data analysis on a Netflix movie dataset containing **9,827 movies** with **9 key features**. The main objective is to clean, preprocess, and analyze the dataset to discover patterns related to **movie genres, popularity, votes, and release trends**.

Through data preprocessing and exploratory data analysis, the project identifies insights about the most common genres, the most popular movies, voting trends, and yearly movie release patterns.

---

## Dataset Preprocessing

Several preprocessing steps were performed to prepare the dataset for analysis.

### Data Cleaning
- Checked for missing values and duplicate records. No missing values or duplicates were found in the dataset.
- Converted the `Release_Date` column into a proper datetime format and extracted the year for time-based analysis.

### Feature Selection
- Removed unnecessary columns including:
  - `overview`
  - `original_language`
  - `Poster_URL`

These columns were not required for the analysis.

### Outlier Detection
- Outliers were identified in the `popularity` column to understand extreme popularity values among movies.

### Vote Average Categorization
The `vote_average` column was categorized into four groups to simplify analysis:

- Popular
- Average
- Below Average
- Not Popular

### Genre Processing
The `Genre` column contained multiple genres in a single field. The following steps were performed:

- Removed extra whitespace from genre values.
- Split multiple genres into separate values.
- Used the explode operation so that each row represents **one genre per movie**.

This transformation makes genre-based analysis more accurate.

---

## Exploratory Data Analysis

Exploratory Data Analysis was conducted to uncover trends and insights from the dataset.

### Most Frequent Genre

Drama is the most frequent genre in the dataset, appearing in approximately **14 percent of all movies**.

---

### Genre with the Highest Votes

About **5.5 percent of movies received a very high number of votes**, which corresponds to approximately **520 records**.

Among all genres, **Drama dominates the voting patterns**, receiving approximately **18.5 times more votes compared to the average genre**.

---

### Most Popular Movie

The most popular movie in the dataset is:

**Spider-Man: No Way Home**

Genres:
- Action
- Adventure
- Science Fiction

---

### Least Popular Movie

The least popular movie identified in the dataset is:

**Threads**

Genres:
- Music
- Drama
- War
- Science Fiction

---

### Year with the Most Movie Releases

The year **2020 recorded the highest number of movie releases** in the dataset.

---

## Technologies Used

The project was implemented using the following technologies:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

These libraries were used for data cleaning, transformation, statistical analysis, and visualization.

---

## Conclusion

This analysis provides useful insights into Netflix movie trends. It highlights patterns in genre popularity, voting behavior, and release trends across different years.

The results show that **Drama is the dominant genre**, and certain blockbuster movies significantly influence popularity metrics.

---

## Author

Palak Sahu  
Bachelor of Technology in Computer Science (AI and ML)

Interested in Machine Learning, Artificial Intelligence, Data Analytics, and Web Development.
