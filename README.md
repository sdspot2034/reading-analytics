# Portfolio Project #1 : Reading Analytics  
## Table of Contents

1. [Introduction: Motivation & Rationale](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#1-introduction-motivation--rationale)
2. [Objectives](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#2-objectives)
3. [Work Samples](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#3-work-samples)  
  3.1. [Dashboard Screenshot](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#31-dashboard-screenshot)  
  3.2. [Key Insights](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#32-key-insights)  
  3.3. [Detailed Analysis](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#33-detailed-analysis)
4. [Data Souce and Connectivity](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#4-detailed-analysis)
5. [Future Scope](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#5-future-scope)
6. [Project Link](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#6-project-link)

---
**Key Focus:**  
<img src="https://upload.wikimedia.org/wikipedia/commons/c/cf/New_Power_BI_Logo.svg" height="40" width="40">  
PowerBI
<br> <br>
**Skill areas:**  
`PowerBI` ; `Data Modelling` ; `Data Cleaning` ; `Data Wrangling` ; `EDA` ; `DAX Expressions` ; `Measures and Calculated Columns` ; `M-Query` ; `Power Query` ; `Data Aggregation`

---

## 1. Introduction: Motivation & Rationale  
> The average person reads approximately **770 books in a lifetime**.  
_Source: [Economic Times](https://www.economist.com/graphic-detail/2023/12/22/how-many-books-will-you-read-before-you-die)_

<br>

> There are roughly **129 million** books in existence.  
_Source: [Google Survey](https://booksearch.blogspot.com/2010/08/books-of-world-stand-up-and-be-counted.html)_

<br>
Thus, the average individual has the opportunity to experience:
<br> <br>

```math
Percentage\ of\ books = (770 * 100) / 129,864,880
```
```math
= 0.00059292396 \ \%
```
<br> <br>
This alarmingly small fraction of accessible literature compelled me to analyze my reading patterns.  
## 2. Objectives:
1. **Optimize book selection** to ensure that choices closely align with personal interests and preferences.
2. **Enhance time management** by concentrating on high-potential books and discontinuing unproductive reads at the appropriate moment.
3. **Minimize the rate of incomplete reads** by ensuring that each book delivers value and aligns with my reading goals and tastes.

## 3. Work Samples:
### 3.1. Dashboard Screenshot
![book analytics high rez](https://github.com/user-attachments/assets/fbc0af80-d229-4130-ba17-f18b6ecd5022)

### 3.2. Key Insights
- Books with average ratings consume the maximum amount of time.
- Books published in earlier periods receive higher ratings and are completed more quickly.
- There is no discernible pattern between the length of a book and the time taken to read it, indicating that reading speed is **not correlated to text volume** and is solely a **function of personal preference**.
- Highly preferred books, on average, take the least time to complete, while books that are less favored tend to be abandoned or shelved sooner.

### 3.3. Detailed Analysis
Graphical representations provide insights and the value derived from this analysis. (Sequence: Top to bottom, then left to right)
#### 3.3.1. Bar Chart - Count of Titles Read by Date
![g1](https://github.com/user-attachments/assets/34c7b60f-f4b7-4e0c-9fe9-978a3c731efe)
- A straightforward graph depicting the trend of completed books by year.
- A bar chart was selected to enhance clarity in the differences.
- **Utility:** Increases motivation to surpass the previous year's count.

#### 3.3.2. Gauge - Count of DNF's by Year
![g2](https://github.com/user-attachments/assets/cfd651a1-0e39-41a1-9631-31789fda2845)
- A gauge chart displaying the number of abandoned books.
- Higher abandonment rates indicate unsuitable book selections and the need for optimization.
- **Utility**: Helps maintain target DNF levels in check to ensure compliance.

#### 3.3.3. Cards - Currently Reading & Last Read
![g3](https://github.com/user-attachments/assets/52e6d8df-644a-46da-9903-832139212fae)
- Cards displaying the most recent book in progress and the last completed book.
- **Utility:** Ensures data freshness and aids in sanity checks.

#### 3.3.4. Bar and Line Chart - Avg Rating, Reading Time by Year of Publication
![g4](https://github.com/user-attachments/assets/df77099e-7b71-4021-835e-15404b983da4)
- The bar chart illustrates the average rating by publication year bucket.
  - Publication years have been categorized into logical buckets of varying sizes.
  - The highest ratings are attributed to books from the earliest eras, demonstrating a clear preference for classics and antiquities.
- The line chart depicts average reading time by publication year bucket.
  - The overlay of the line chart on the bar graph reveals correlations between the two metrics.
  - Books from earlier periods are read the fastest.
- The dual-axis design ensures clarity in correlation and consistency in the visual range.
- **Utility:** Highlights the relationship between the preferred publication period, rating, and reading time.

#### 3.3.5. Line Graph - Reading Time by Number of Pages
![g5](https://github.com/user-attachments/assets/1a57c3bd-8c10-4e70-ae77-96a12aea8cf5)
- No clear correlation exists between book length and reading time.
- Reading speed is independent of book volume.
- **Utility:** Emphasizes the relevance of reading time concerning text density.

#### 3.3.6. Line Chart - Average Reading Time in Days by Rating
![g6](https://github.com/user-attachments/assets/d9786e33-0c2c-4ba7-b4bc-581731518ff4)
- The law of diminishing marginal returns is observed.
- Books with above-average ratings, but not in the highest preferred zone (> 4-star rating), exhibit the longest reading times.
- **Utility:** Enables early identification of time-consuming books.

#### 3.3.7. Scatter Plot - Reading Time vs. Rating: Correlation and Distribution
![g7](https://github.com/user-attachments/assets/b3823a0e-64da-44d8-a271-e5d536941ccc)
- Scatter plot displaying data points across ratings.
- The size of the bubbles indicates the number of pages in each title.
- The visual can be divided into four quadrants:
  1. < 3 and < 50: Poorly rated books are either finished or abandoned quickly.
  2. < 3 and > 50: No poorly rated books lasted long.
  3. <span>>=</span> 3 and < 50: Majority distribution of quickly finished books with ratings exceeding 4.
  4. <span>>=</span> 3 and > 50: A single book with an average rating and very high length skews data outputs in average calculations. Most other averagely rated books were finished in a timely manner, with only a few taking longer.
- **Utility:** Distribution plots help debunk inaccurate insights in averages caused by outliers.

## 4. Data Source and Connectivity:
Data Source: 
- Personal records of reading activities through Aug'21 - Present.
- This was maintained in a Google Sheets Workbook segregates into worksheets by year.
- OAuth was used to allow data access from personal drive.
- Appending of all worksheets into a single table was performed with **M-Query** in Power Query Data Source Advanced Settings.

## 5. Future Scope:
1. Geographical analysis of author origins.
2. Integration of insights related to book genres and their likability.

## 6. Project link:
[PowerBI Published Link](https://app.powerbi.com/groups/me/reports/a640585b-4ab6-4e54-b411-fc9d4ea189d6/ReportSectionc7cb1c9a71a71512454b?redirectedFromSignup=1&experience=power-bi
