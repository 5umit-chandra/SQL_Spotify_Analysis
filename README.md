# 🟢 Most Streamed Spotify Songs 2023 - SQL Analysis

## 📝 Project Overview
### Introduction
Explore the dynamic music landscape of 2023 through advanced SQL queries on the "Most Streamed Spotify Songs" dataset. Uncover artist trends, temporal patterns, and the relationship between song attributes and popularity.

### Key Features
1. **Most Listened-to Artists**
   - The Weeknd, Taylor Swift, and Ed Sheeran dominate total streams, showcasing global popularity.

2. **Song Counts Released Annually**
   - Explore the evolving music industry landscape with a detailed breakdown of song releases by year, spanning from the 1950s onwards.

3. **New Songs**
   - Stay current with a curated list of the latest songs in 2023, providing valuable insights for music enthusiasts and industry professionals.

4. **Most Popular Songs on Spotify and Apple Music**
   - Identify current musical trends and preferences across major streaming platforms, including ranks and popularity metrics.

5. **High-Tempo Songs**
   - Catering to energetic listeners, discover a list of high-tempo songs with beats per minute (BPM) over 150.

6. **Songs Found in Most Playlists**
   - Shed light on user playlist preferences with an identification of songs frequently found in Spotify and Apple Music playlists.

7. **Energetic Songs**
   - Explore a curated list of energetic songs with a high energy percentage for dynamic musical experiences.

8. **Acoustic Songs**
   - Discover non-acoustic or minimally acoustic tracks with a low acoustic ratio (acousticness percentage < 10).

9. **Songs with High Lyrical Content**
   - Catering to lyric enthusiasts, identify songs with high lyrical content based on a speechiness percentage > 10.

## 📊 Data Analysis
The SQL queries for data analysis are consolidated in the main file, [SQL_queries.sql](SQL_queries.sql), providing a granular exploration of the dataset. These analyses offer a multifaceted view of the music industry in 2023, covering user preferences, artist impact, and song attributes.

## 🧠 Conclusions
The findings from this SQL analysis offer actionable insights into the dynamic music landscape of 2023. Top artists, trends in annual song releases, and characteristics of popular songs provide a comprehensive understanding of the industry. This knowledge can guide strategic decisions for artists, platforms, and industry stakeholders.

## ℹ️ Dataset Source
The initial raw dataset is downloaded in CSV format from [Kaggle.com](https://www.kaggle.com/). The dataset is stored in the file [spotify-2023.csv](MySQL Schemea and Data\spotify-2023.csv).

## 💾 Raw Data
To facilitate analysis, the dataset was imported into MySQL. The schema for the MySQL database is defined in [Schemea.sql](link to file), and the data is loaded into the table using [spotify_2023_spotify_data.sql](MySQL Schemea and Data\spotify_2023_spotify_data.sql).

## 👨‍💻 Data Import Process
1. **Download Raw Dataset:**
   - The initial dataset was obtained as a CSV file from Kaggle.

2. **MySQL Schema Definition:**
   - The schema for the MySQL database is defined in [Schemea.sql](MySQL Schemea and Data\Schemea.sql).

3. **MySQL Data Import:**
   - Utilize the "Table Data Import Wizard" or use the provided SQL query in [spotify_2023_spotify_data.sql](MySQL Schemea and Data\spotify_2023_spotify_data.sql) for efficient data import.

```sql
-- Example import query
LOAD DATA INFILE 'MySQL Schemea and Data\spotify-2023.csv'
INTO TABLE spotify_data
-- Specify field delimiter in CSV
FIELDS TERMINATED BY ','
-- encloser fields containing text
ENCLOSED BY '"'
LINES TERMINATED BY '\n'
-- skips the first row of CSV
IGNORE 1 ROWS;
```