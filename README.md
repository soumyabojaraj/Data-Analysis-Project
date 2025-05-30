# 📚 Amazon Bestselling Book Analysis

## Goal

**What kind of book sells well on Amazon’s self-publishing platform?**

---

## Libraries Used

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

---

## Dataset Used

- **Source**: [Amazon Top 50 Bestselling Books (2009–2019) – Kaggle](https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019)
- **Year Analyzed**: 2024 version
- **Shape**: 4846 rows × 10 columns

---

## Initial Observations

- Missing values in **`Brand`** and **`Number of Pages`** columns
- Outliers detected in the **`Number of Pages`** column

---

## Data Cleaning Steps

- Dropped the **`Brand`** column
- Removed rows with missing **`Number of Pages`**
- Removed outliers based on page count
- Renamed **`Reviews`** column to **`Ratings`**

🔹 **Final Dataset Shape**: 4710 rows × 9 columns

---

## Key Insights

- **Top-Selling Genres**: *Fantasy*, *Classics*, and *Motivational*
- **Average Page Count**: ~313 pages
- **Optimal Price Range**: $10–$15
- **Successful Genre Traits**:
  - High ratings (~4.8)
  - High review counts (~5,000+)
- **Price vs. Ratings/Reviews**: No strong correlation found

---

## Recommendations

| Aspect       | Recommendation                                  |
|--------------|--------------------------------------------------|
| **Genre**     | Focus on *Fantasy*, *Classics*, *Motivational*  |
| **Page Count**| Aim for **300–320 pages**                       |
| **Price**     | Set between **$10 and $15**                     |
| **Ratings & Reviews** | Include inserts, engage with reader communities |

---

## Limitations

- No way to distinguish between **self-published** vs **traditionally published** books
- **Format data** (e.g., paperback, Kindle, audiobook) is missing
- No information on book **dimensions**, **printing requirements**, or **release year**

---

## Future Scope

- Analyze **Author** popularity vs. sales performance
- Compare **Manufacturers** for pricing patterns

---

## Citations

- **Dataset**: [Kaggle – Amazon Top 50 Bestselling Books (2009–2019)](https://www.kaggle.com/datasets/sootersaalu/amazon-top-50-bestselling-books-2009-2019)
- **Markdown Styling**: [Markdown Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
- **Visualizations**:
  - [Vertical Lines in Distplot – StackOverflow](https://stackoverflow.com/questions/52334938/how-to-add-vertical-lines-to-a-distribution-plot)
  - [Matplotlib Pie Charts – W3Schools](https://www.w3schools.com/python/matplotlib_pie_charts.asp)
  - [Seaborn Heatmap](https://seaborn.pydata.org/generated/seaborn.heatmap.html)
  - [Seaborn Scatterplot](https://seaborn.pydata.org/generated/seaborn.scatterplot.html)
