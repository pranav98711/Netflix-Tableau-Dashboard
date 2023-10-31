# Netflix-Tableau-Dashboard


## Data Import:

The project begins with the import of a [CSV files]([https://pages.github.com/](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Dataset/netflix_titles.xls)) containing Netflix data, which includes 12 fields and over 6,000 rows. The fields include information like show ID, type (movie or TV show), titles, directors, cast, date added, release year, rating, duration, categories, and descriptions. Tableau automatically recognizes the data fields and structures them accordingly.
Tableau's data preparation capabilities, including data cleansing and transformation, can be employed to handle null values, correct data types, and ensure data integrity. However, the data is pretty clean, adapted for using in Tableau, so not much preprocessing is required. There is no problematic outliers either. 
Here are some screenshots of the Data Source Page. The Fields section shows the different parameters present in our data.

![](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Images/data_1.png)

This other screenshot shows the sample 100 rows from dataset with their values.

![](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Images/data_2.png)
![](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Images/data_3.png)

## Initial Data Analysis:

### Total Movies and TV Shows by Year:

![](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Images/1.png)

The initial visualization involves creating a time series chart by placing the "Date Added" field in the Columns shelf and the "Show ID" field in the Rows shelf as a count distinct measure.
Null values within the "Release Year" field can be filtered out using a filter action and then applied.
The chart is transformed into an area chart with specific formatting adjustments, such as black background and red text, through Tableau's chart properties.

### Geographical Analysis:

![](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Images/2.png)

The map visualization is established by placing the "Country" field on the Rows shelf and applying a color encoding based on a measure (e.g., count of Show IDs).
Tableau's mapping features can be used to define geographical roles and customize map colors and tooltips for enhanced presentation.

### Top 10 Genres:

![](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Images/3.png)

The top 10 genres are identified using calculations and placed in a bar chart, presenting a ranked view of content genres.

### Ratings Analysis:

![](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Images/5.png)

A histogram-like chart is created by placing the "Ratings" field on the Rows shelf and utilizing measures (e.g., count of Show IDs) to visualize the distribution of content ratings.

### Descriptive Information:

![](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Images/7.png)

Individual content details, such as descriptions, date added, duration, ratings, release year, and genres, are incorporated by placing the corresponding fields in a Tableau dashboard. The data is dynamically filtered based on user interaction.

## Dashboard Creation:

![](https://github.com/pranav98711/Netflix-Tableau-Dashboard/blob/main/Images/6.png)

The Netflix dashboard is crafted by integrating multiple worksheets as previously detailed into a cohesive interface. Interactive filters are thoughtfully incorporated, affording users control over their data exploration. These filters are designed by incorporating distinct fields such as "Type" and "Titles" within the dashboard.

When a specific content type and title are selected, the dashboard dynamically presents the associated details including Description, Date Added, Duration, Rating, Release Year, Genre, and more. In addition to this individual content view, the dashboard also offers a comprehensive summary encompassing the aggregate counts of movies and TV shows over different years and geographical regions. It also highlights the top content genres and other key insights.

This design empowers users to seamlessly navigate and delve into the Netflix dataset while maintaining a holistic view of the dataset's characteristics, facilitating a richer understanding of the content library.








