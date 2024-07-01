## 🔗 Links
| Work   | Owner             | Presentation                                            |
| :-------------| :--------------- | :----------------------------------------------------- |
|[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://github.com/rajbhuwan1510/)| [![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rajbhuwan-jaitawat/)| [![Microsoft PowerPoint](https://img.shields.io/badge/Microsoft_PowerPoint-B7472A?style=for-the-badge&logo=microsoft-powerpoint&logoColor=white)](https://docs.google.com/presentation/d/1Nm-RP4LRsWzELmdVWoL_7LVz67Sx2xoCGu53aKcVxH0/edit#slide=id.g2710a2587c9_1_1438)

# Netflix Content Analysis Project


## Overview

Welcome to the Netflix Content Analysis Project! This project aims to analyze various aspects of Netflix's extensive library, including the growth of movies and TV shows, genre distribution, country of origin, content duration, rating categories, release patterns, director and cast involvement, genre popularity over time, and much more.

## Project Structure

- Get data from here [![Kaggle](https://img.shields.io/badge/Kaggle-035a7d?style=for-the-badge&logo=kaggle&logoColor=white) ](https://www.kaggle.com/datasets/ariyoomotade/netflix-data-cleaning-analysis-and-visualization)
- Contains datasets used for analysis. [![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/blob/main/Netflix_project.ipynb)
    - Jupyter notebooks containing code for data analysis.

- `results` **Genereated by WorldCloud**![walpaper](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/9fdf0301-da6c-40bd-a5e2-018d267ffa59)


## Data Cleaning

In this project, comprehensive data cleaning was performed to ensure the quality and integrity of the dataset. The cleaning process involved several steps aimed at standardizing and preparing the data for analysis.

1. **Standardizing Date Formats:**
   - The `release_date` column was converted into a standardized date format to facilitate easier analysis.
   - Additionally, a consistency check was implemented to ensure that the `release_date` does not exceed the `added_date`. Any discrepancies found were addressed by dropping the corresponding data entries, ensuring data accuracy.

2. **Handling Multi-Value Columns:**
   - Columns such as `cast`, `listed_in`, `country`, and `director` often contained multiple values separated by commas. To facilitate better analysis, these columns were transformed into lists, allowing for easier parsing and exploration of the data.
   - Furthermore, missing values in these columns were addressed by filling them with appropriate placeholders to maintain data integrity.

3. **Correcting Misplaced Data:**
   - During the data cleaning process, instances were identified where data was mistakenly placed or entered in incorrect columns. These errors were rectified to ensure the accuracy and consistency of the dataset.
   - By conducting thorough checks and validations, such discrepancies were identified and corrected, enhancing the reliability of the dataset for further analysis.
   
### Data Understanding

- Number of rows and columns: [8807,12]

| Column name   | Type             | Description                                            |
| :-------------| :--------------- |:----------------------------------------------------- |
| `show_id`     | `object`         | A unique identifier for each title.|
| `type`        | `object`         | The category of the title, which is either 'Movie' or 'TV Show'.|
| `title`       | `object`         | The name of the movie or TV show.|
| `director`    | `object`         | The director(s) of the movie or TV show.              |
| `cast`        | `object`         | The list of main actors/actresses in the title.       |
| `country`     | `object`         | The country or countries where the movie or TV show was produced. |
| `date_added`  | `object`         | The date the title was added to Netflix.              |
| `release_year`| `datetime64[ns]` | The year the movie or TV show was originally released. |
| `rating`      | `object`         | The age rating of the title.                          |
| `duration`    | `int`            | The duration of the title, in minutes for movies and seasons for TV shows. |
| `listed_in`   | `object`         | The genres the title falls under.                     |
| `description` | `object`         | A brief summary of the title.                         |




## Data Exploration and Visualization

- Created histograms to visualize the distribution of numerical features.
- Visualized the distribution of categorical features using bar charts or pie charts.
- Used boxplots to compare distributions across different groups or categories.
- Explored relationships between variables using scatter plots or correlation matrices.
- Employed Seaborn for more advanced visualizations like pairplots, heatmaps, etc.

## Insights and Conclusion

- Key findings from the EDA, including patterns or relationships discovered.

- Drawn many interesting inferences from the dataset Netflix titles; here’s a summary of the few of them:

- The most content type on Netflix is *`Movies`*.

- The country by the amount of the produces content is the *`United States`*,

- The most popular director on Netflix , with the most titles, is *`Rajiv Chilaka`*.

- *`International Movies`* is a genre that is mostly in Netflix.

- largest count of Netflix content is made with a *`TV-MA`* rating.

- The most popular actor on Netflix movie, based on the number of titles, is *`Anupam Kher`*.

## Questions Explored

1. Growth of Movies and TV Shows
![CategoryVSyear](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/50c593bd-0c44-475b-aa04-12d3640a543e)

2. Distribution of Genres
![Different GenreDistribution](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/3d298930-3415-427b-a5ef-507614219e5a)

3. Distribution by Country of Origin![countries](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/e90aa3eb-8d79-4fd7-b0e8-75027cd452a7)

4. Content Duration over Years
![durationOverYear](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/12f28298-fc12-4ea7-a50c-b24f8c355c6a)

5. Distribution by Rating Categories
![Distribution of Content Across Different Rating Categories](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/bbe23494-2105-4907-b9ef-3a32471c8977)

6. Volume of Releases Over Time
- Movies
![Movies distribution over time](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/8b670250-3af6-45f6-8339-837bdb97d905)
- TV Shows
![Distribution of TV Shows Durations histplot](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/802cb8a0-c1b6-4784-ac09-0d29be031ef5)

7. Content Addition Activity Over Months/Quarters![Content Addition Activity Over MonthsQuarters](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/6519c404-4d8e-4209-8135-feb05cb45c23)

8. Patterns in Release Dates
![CategoryVSyear](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/1506580f-3302-4e49-b93a-2c15b169074e)

9. Frequent Directors and their Content Contribution![top 10 director](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/8cce1f24-c914-46a7-b5bf-9661a9ea693f)

10. Frequent Cast Members and their Involvement![top 10 cast](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/4a9d3bf1-0f69-4f42-8d40-bd525870b3c0)

11. Changes in Genre Popularity Over Time
- Movies![Popularity of Genres Over Time for movies](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/a41de859-012e-4da2-b7e4-de16a29fdaab)
- TV Shows![Popularity of Genres Over Time for TV Shows](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/6e951cf0-5726-4558-b123-dea1bfed8bd7)

12. Relationship Between Content Duration and Rating
![Different GenreDistribution](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/2c94f8cd-1494-4586-9607-ece872ffe40f)


13. Correlation Between Rating and Country of Origin
![countryVgenre](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/cbe9a620-6fc5-4c9a-a1e3-28cb5f9061b6)


14. Director-Genre Associations
![country_genre_visual (2)](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/5dc123b0-9580-43fa-b34c-f8db95bafce4)

15. Cast-Genre Associations
![CastVSgenre](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/96f7d3d8-4021-4e48-9c75-236d476911aa)

16. Co-occurrence of Genres
![Genre count](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/684dfcd2-2ec4-4cc0-9982-8ecc4ab28ecf)


![relationBetweenGenereandcount2](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/06cf604a-2cef-4547-9d2a-9bc8e6b0c5bb)


17. Evolution of Content Themes Over Time![Popularity of Genres Over Time](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/ffd2077f-11b6-4831-9e08-81750b2ea32a)


18. Comparison Between Original and Licensed Content
![netflix orignal or not](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/87d3b8c1-61e4-48f2-8893-26a5e72d8f1a)

19. Changes in Diversity of Content Over Time
![GenreVSratingVScountry](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/328392d2-71f5-4eaf-a671-8f2209f74591)

20. Correlation Between Age of Content and Popularity/Rating
![audience guidence violen](https://github.com/rajbhuwan1510/NetFlixDataAnalysis/assets/92216824/315dda31-765f-4671-b5f4-e315ceefd330)


## Technologies Used

- Python
- Pandas
- Numpy
- Matplotlib
- Seaborn
- itertools
- Statistics
- Jupyter Notebook
