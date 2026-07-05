# Netflix Data Analysis Report

## 1. Introduction

Netflix has become one of the world's leading streaming entertainment platforms, offering a vast and diverse catalog of movies and television shows to millions of subscribers globally. Understanding the composition, growth patterns, and strategic positioning of this content library provides valuable insight into the platform's content acquisition strategy and competitive positioning within the streaming industry. This report presents a comprehensive data analysis of Netflix's content catalog, covering data cleaning methodology, exploratory analysis, visualization, and actionable business insights.

## 2. Objective

The primary objective of this analysis is to explore the Netflix Movies and TV Shows dataset to uncover patterns related to content type distribution, geographic concentration, genre popularity, content growth over time, and audience targeting through content ratings. The analysis aims to translate these patterns into meaningful business insights relevant to content strategy and competitive positioning.

## 3. Dataset

The dataset used for this analysis is the "Netflix Movies and TV Shows" dataset sourced from Kaggle. It contains 8,807 records across 12 attributes, including show identifier, content type, title, director, cast, country of production, date added to the platform, release year, content rating, duration, genre classification, and description.

## 4. Methodology

The analysis followed a structured data analytics workflow comprising problem understanding, data collection, data cleaning, exploratory data analysis, visualization, and insight generation. Python was used as the primary analytical tool, leveraging the Pandas library for data manipulation and Matplotlib for visualization, within a Jupyter Notebook environment.

## 5. Data Cleaning Process

Initial inspection revealed missing values across several columns: director (29.91%), country (9.44%), and cast (9.37%), alongside minor gaps in date_added, rating, and duration (each under 0.15%). Given the substantial proportion of missing data in director, cast, and country, these fields were imputed with "Unknown" rather than removed, preserving the integrity of the broader dataset. Rows with missing values in date_added, rating, and duration—representing a negligible fraction of total records—were removed, as imputing such values risked introducing inaccuracies into time-based and categorical analyses. Additional cleaning steps included stripping extraneous whitespace from text fields, converting date_added to a proper datetime format, and standardizing text casing for consistency. A new year_added column was derived to facilitate temporal analysis. No duplicate records were identified in the dataset.

## 6. Analysis

Exploratory analysis addressed fourteen key business questions spanning content composition, geographic distribution, genre trends, ratings, growth trajectory, and talent contributions. Movies constitute approximately 70% of the catalog, with television shows comprising the remaining 30%. The United States dominates as the leading production country, followed by India and the United Kingdom. Dramatic and international genre categories, along with documentaries and stand-up comedy, emerged as the most prevalent content classifications. Content additions grew substantially between 2016 and 2019, peaking at nearly 2,000 titles annually, before declining in 2020 and 2021.

## 7. Visualizations

Six visualizations were developed to support the analysis: a bar chart comparing movie and television show counts, a horizontal bar chart of the top ten content-producing countries, a line chart depicting content growth over time, a bar chart of content rating distribution, a histogram of movie duration, and a pie chart of the top five genre classifications. These visualizations are available in the accompanying visuals directory.

## 8. Key Insights

Four primary insights emerged from this analysis. First, Netflix's content strategy exhibits a pronounced film-centric orientation, which may understate the engagement benefits associated with episodic television content. Second, the catalog demonstrates significant geographic concentration in U.S.-produced content, though growing investment in Indian content signals a strategic pivot toward high-growth international markets. Third, the platform's content acquisition trajectory reflects a shift from aggressive volume-driven growth toward a more selective, quality-focused strategy, likely in response to intensifying competition. Fourth, the concentration of mature-rated content suggests a deliberate targeting of adult and young-adult audiences, potentially at the expense of deeper penetration into family-oriented market segments.

## 9. Recommendations

Based on these findings, it is recommended that Netflix consider increasing investment in television series production to strengthen subscriber retention through sustained engagement. Expanding regionally diverse content, particularly in high-growth markets beyond the United States, may support deeper international market penetration. Improving data governance practices around country and director attribution would enhance the precision of future content-strategy analyses. Finally, diversifying the content ratings mix could help capture a broader family-oriented audience segment increasingly targeted by competing platforms.

## 10. Conclusion

This analysis demonstrates that Netflix's content catalog reflects a deliberate, evolving strategy shaped by competitive pressures and international expansion goals. While the platform maintains a strong film-centric and U.S.-concentrated content base, emerging patterns in geographic diversification and content-type balance suggest ongoing strategic adaptation. Continued data-driven monitoring of content composition will remain essential for sustaining competitive advantage in an increasingly crowded streaming market.