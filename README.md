# Portfolio Project #1 : Reading Analytics  
## Table of Contents

1. [Introduction: Motivation & Rationale](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#1-introduction-motivation--rationale)
2. [Objectives](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#2-objectives)
3. [Work Samples](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#3-work-samples)  
  3.1. [Dashboard Screenshot](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#31-dashboard-screenshot)  
  3.2. [Key Insights](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#32-key-insights)  
  3.3. [Detailed Analysis](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#33-detailed-analysis)
4. [Future Scope](https://github.com/sdspot2034/reading-analytics/blob/main/README.md#4-future-scope)

## 1. Introduction: Motivation & Rationale  
> The average person reads about **770 books in a lifetime**.  
_Source: [Economic Times](https://www.economist.com/graphic-detail/2023/12/22/how-many-books-will-you-read-before-you-die)_

<br>

> There are roughly **129 million** books in the world.  
_Source: [Google Survey](https://booksearch.blogspot.com/2010/08/books-of-world-stand-up-and-be-counted.html)_

<br>
Therefore, an average person would only get to experience:
<br> <br>

```math
Percentage\ of\ books = (770 * 100) / 129,864,880
```
```math
= 0.00059292396\ \%
```
<br> <br>
This frighteningly small fraction of books at my disposal to be consumed galvanized me into analysing my reading patterns.  
## 2. Objectives:
1. **Optimize book selection** to ensure choices align closely with personal interests and preferences.
2. **Enhance time management** by focusing on high-potential books and discontinuing unproductive reads at the right moment.
3. **Minimize the rate of incomplete reads** by ensuring each book delivers value and aligns with my reading goals and tastes.

## 3. Work Samples:
### 3.1. Dashboard Screenshot
![book analytics high rez](https://github.com/user-attachments/assets/fbc0af80-d229-4130-ba17-f18b6ecd5022)


### 3.2. Key Insights
- Books with average rating consume maximum amount of time.
- Books written in the earlier periods are rated higher and take fastest amount of time to complete.
- No clear pattern between length of book and amount of time taken indicates the reading speed is **not correlated to text volume** and is only a **direct and sole function of preference**
- Highly preferred books on average take the least amount of time. While highly disliked books show potential to be concluded/shelved sooner.

### 3.3. Detailed Analysis
Graph-wise explanation of insights and value obtained. (Sequence: Top to bottom, then left to right)
#### 3.3.1. Bar Chart - Count of Titles Read by Date
![g1](https://github.com/user-attachments/assets/34c7b60f-f4b7-4e0c-9fe9-978a3c731efe)
- A simple graph depicting trend of completed books by year.
- A bar chart was chosen so as to increase clarity in differences.
- **Utility:** Boosts drive to beat previous year's count.

#### 3.3.2. Gauge - Count of DNF's by Year
![g2](https://github.com/user-attachments/assets/cfd651a1-0e39-41a1-9631-31789fda2845)
- A gauge chart showing count of books abandoned.
- Higher abandonment rates indicate unsuitable selection of books and need for optimisation.
- **Utility**: Keeping target value of DNF in check and ensure compliance.

#### 3.3.3. Cards - Currently Reading & Last Read
![g3](https://github.com/user-attachments/assets/52e6d8df-644a-46da-9903-832139212fae)
- Cards showing latest book in progress and last completed book.
- **Utility:** Sanity testing and data freshness

#### 3.3.4. Bar and Line Chart - Avg Rating, Reading Time by Year of Publication
![g4](https://github.com/user-attachments/assets/df77099e-7b71-4021-835e-15404b983da4)
- Bar chart shows average rating by publication year bucket.
  - Publication year of books has been broken into logical buckets of varying sizes.
  - Highest ratings were provided to books of the earliest epoch, showing a clear proclivity to the classics and antiques.
- Line chart shows average reading time by publication year bucket.
  - Superposition of line chart over bar graph reveals correlations between the two metrics.
  - Books written in the earliest eras have been read the fastest.
- Dual axis ensures clarity in correlation and consistent range of the visual.
- **Utility:** Highlights correlation between preferred time period of book and rating along with reading time.

#### 3.3.5. Line Graph - Reading Time by Number of Pages
![g5](https://github.com/user-attachments/assets/1a57c3bd-8c10-4e70-ae77-96a12aea8cf5)
- No clear correlation between length of book and reading time.
- Reading speed is independent of volume of book.
- **Utility:** Highlights relevance of reading time with respect to text density.

#### 3.3.6. Line Chart - Average of Reading Time in days by Rating
![g6](https://github.com/user-attachments/assets/d9786e33-0c2c-4ba7-b4bc-581731518ff4)
- Law of diminishing marginal returns observed.
- Books with above average rating, but not in the most liked zone (> 4 star rating) show highest time in reading.
- **Utility:** Early pre-emption of time-consuming books.

#### 3.3.7. Scatter Plot - Reading Time v Rating: Correlation and Distribution
![g7](https://github.com/user-attachments/assets/b3823a0e-64da-44d8-a271-e5d536941ccc)
- Scatter of data points across ratings.
- Size of bubbles indicate number of pages in title.
- Visual can be divided into 4 qudrants:
  1. < 3 and < 50: Books poorly-rated were either finished or abandoned post-haste
  2. < 3 and > 50: No book poorly-rated lasted long.
  3. <span>>=</span> 3 and < 50 : Majority distribution of fast-finished books with ratings higher than 4.
  4. <span>>=</span> 3 and > 50: Single book with average rating and very high length has skewed data outputs in average calculations. Most other books averagely rated were finished in due time. Rare few books took long.
- **Utility:** Distribution plots help in debunking inaccurate insights in averages caused due to outliers.


## 4. Future Scope
1. Geographical view of Author origin.
2. Incorporation of insights into genres of books and likeability.
