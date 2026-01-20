
# Lab 2: Web Data Collection and Visualization

**Course:** GEOG 458
**Instructor:** Bo Zhao
**Student:** Malaika

---

## 1. Research Topic and Search Parameters

The goal of this lab is to explore how YouTube users discuss topics related to the University of Washington by collecting and analyzing video metadata using a web crawler. To capture variations in how the same topic is referenced, I ran the YouTube crawler using the following three search terms:

* **"uw"**
* **"university of washington"**
* **"univ of washington"**

Each search term was executed separately using the same crawler logic to ensure consistency across datasets. The crawler collected video metadata including titles, short descriptions, view counts, upload times, and collection timestamps. The resulting datasets were exported as CSV files and stored in the repository.

---

## 2. Motivation for the Comparison

The motivation behind using multiple search terms is that users often refer to the same institution in different ways. A single keyword search may fail to capture the full range of discourse. By comparing results from abbreviated, formal, and semi-formal search terms, this analysis aims to understand whether different naming conventions lead to different thematic emphases or narratives on YouTube.

This comparison helps evaluate how keyword selection influences data collection outcomes in web-based research.

---

## 3. Word Cloud Comparison and Analysis

To analyze the content of the collected videos, word clouds were generated using the `shortdesc` field from each dataset. These word clouds visualize the most frequently occurring terms and provide a high-level summary of discussion themes.

### Word Cloud: "uw"

![UW Word Cloud](img/wordcloud-uw.png)

### Word Cloud: "university of washington"

![University of Washington Word Cloud](img/wordcloud-university.png)

**Comparison:**
The word cloud generated from the search term **"uw"** shows a higher frequency of informal and student-oriented terms, including references to campus life, sports, and student experiences. In contrast, the **"university of washington"** word cloud emphasizes more formal language, including academic programs, research, and institutional branding.

Despite these differences, both word clouds share common terms related to education and campus identity, indicating a shared underlying topic with variations in emphasis.

---

## 4. Possible Explanations for Observed Patterns

The observed differences likely stem from the audiences using each term. Shortened terms such as "uw" are commonly used by students and alumni, which may explain the prevalence of informal and community-focused language. The full institutional name, on the other hand, is more likely used in official content, news coverage, and academic contexts.

Additionally, YouTube’s recommendation and ranking algorithms may surface different types of videos depending on the specificity of the search query.

---

## 5. Limitations and Future Improvements

This analysis has several limitations:

* The data represents a snapshot in time and does not account for temporal trends.
* The crawler only collected a limited number of videos per search term.
* Word clouds emphasize frequency but do not capture sentiment or context.

Future improvements could include:

* Running the crawler at multiple time points
* Increasing the number of scrolls to collect larger datasets
* Applying natural language processing techniques such as topic modeling or sentiment analysis
* Expanding the study to include geographic filtering or channel-level analysis

---

## 6. Unexpected Observations

One unexpected observation was the degree to which informal search terms surfaced highly viewed and widely shared content, suggesting that abbreviated keywords may play a significant role in content discoverability on YouTube. This highlights the importance of thoughtful keyword selection when conducting web-based data collection.

---

## 7. Data Access

The collected datasets can be downloaded from the links below:

* [uw.csv](assets/uw.csv)
* [university_of_washington.csv](assets/university_of_washington.csv)
* [univ_of_washington.csv](assets/univ_of_washington.csv)

---

## 8. Conclusion

This lab demonstrates how web crawlers can be used to collect and visualize online data, and how small changes in search parameters can lead to meaningful differences in analytical outcomes. The results emphasize the importance of methodological choices in web data research and provide a foundation for more advanced spatial or thematic analyses in future work.
