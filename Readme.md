# Project

## Task 1

You’re interested in understanding the productivity of contributors on reddit.org. For this analysis, you first need to:

- scrape the Reddit posts for a given subreddit (e.g., “r/emacs”) within a given period (e.g., “01/2023-03/2023”)
- extract for each post 5 important metrics (up to you to choose)
- generate a CSV file with one line per post, where each line contains an identifier for a post and the values for the 5 chosen metrics

Then, perform an initial analysis where you obtain the CSV file for two subreddits (e.g., “r/emacs” and “r/vim”) within 3 months (e.g., “01/2023-03/2023”). You should:

- generate plots to understand the differences in the distribution of the 5 metrics across the two subreddits

## Task 2

Add an additional type of analysis that could provide a better understanding of differences in contributor behavior between both subreddits

- Sentimental Analysis
- Word Frequency Analysis
- Emoji Analysis

# Directory Layout

<pre>
.
├── Reddit Scraping Project
|      ├── Task_1.ipynp
|      ├── Sentimental_Analysis.ipynb
|      ├── Word_Freq_Analysis.ipynb
|      └──CSV Files
|           ├── Scrape_vr_final.csv
|           ├── Scrape_wd_final.csv
|           ├── Headlines_vr.csv
|           ├── Headlines_wd.csv
|           ├── SAR_headline_vr.csv
|           └── SAR_headline_wd.csv
</pre>

# Metrics

| Parameter      | Type     | Description                                                         |
| :------------- | :------- | :------------------------------------------------------------------ |
| `Number`       | `int`    | Row numbering                                                       |
| `Id`           | `object` | ID of the submission                                                |
| `Title`        | `object` | Title of the submission                                             |
| `Upvotes`      | `int`    | Number of upvotes for the submission (Score)                        |
| `Upvote Ratio` | `float`  | Percentage of upvotes from all votes on the submission              |
| `Comments`     | `int`    | Number of comments on the submission                                |
| `Timestamp`    | `object` | Time the submission was created                                     |
| `Total Votes`  | `int`    | Total number of votes (Total Votes = Upvotes / Upvote Ratio)        |
| `Downvotes`    | `int`    | Total number of downvotes (Downvotes = Total Votes - Upvotes)       |
| `Engagement`   | `int`    | Shows the trend in engagement (Engagement = Total Votes + Comments) |

# Python Libraries Used

| Library             | Description                                                      |
| :------------------ | :--------------------------------------------------------------- |
| `pprint`            | For better readability of data structures                        |
| `pandas`            | For data manipulation and analysis                               |
| `numpy`             | For numerical computations                                       |
| `matplotlib.pyplot` | For creating visualizations                                      |
| `seaborn`           | For statistical data visualization                               |
| `praw`              | For simple access to Reddit's API                                |
| `datetime`          | To create, manipulate, and format dates and times                |
| `nltk`              | For sentiment analysis                                           |
| `stopwords`         | To remove common words that are not important like to, the, etc. |
| `word_tokenize`     | To break text into words                                         |
| `WordNetLemmatizer` | For word lemmatization                                           |
| `Counter`           | For counting hashable objects                                    |
| `emoji`             | For handling emojis                                              |

# App Creation

- Create a reddit account.
- Create an app on "https://www.reddit.com/prefs/apps".
- Add `Name`, select `script` for personal use and give a `redirect uri`. Use "http://localhost:8080" for `redirect_uri`.
- Copy `client_id` and `client_secret` to use it while creating a reddit instance.

# References

- [Create App](https://www.reddit.com/prefs/apps)
- [PRAW Documentation](https://praw.readthedocs.io/en/latest/index.html)
- [Time Format Conversion](https://www.unixtimestamp.com/index.php)

# Author

[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://aham18113.vercel.app/)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aham-gupta-18a02a202/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/aham-18113)
[![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ahamgupta18113@gmail.com)
