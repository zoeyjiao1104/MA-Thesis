# MA-Thesis

`Reddit_data.ipynb` is a notebook for scraping Reddit data from the following subreddits **lactoseintolerant** , **lactoseintolerance** , **milkmemes** , **AncestryDNA** , **23AndMe** , **MyHeritage**. All posts and comments are scraped from each subreddits. For the first three subreddits, the posts are combined into a dataframe and the comments are combined into a dataframe, which I named as **lactose_df_posts** and **lactose_df_comments** because these three subreddits are related to lactose. The other three subreddits are combined into another dataframe (posts and comments separated), named as **genome_df_posts** and **genome_df_comments** for they are related to genetics. After some data cleaning, there are 6,992 posts and 41,813 comments in the lactose dataframe; 25,852 posts and 768,767 comments in the genome dataframe. 

`Exploratory Analysis.ipynb` is a notebook for exploring the datasets. I am going to analyze the lactose_df and the genome_df separately. First of all, I would like to count the number of words related to 'race' and 'genes' appearing in the lactose_dfs. On the other hand, I would like to count the number of words related to 'lactose' appearing in the genome_dfs. I did the word count, as well as identify the original posts/comments that the word appear (exported into csv for further interpretation). It turns out that a significant number of race-related words (2809 times) appear in the lactose_dfs and the same happend to lactose-related words (236 times) in the genome_dfs. This finding suggests that lactose and genetics are closely associated in these subreddit discourses. 
Next, I ran LDA topic modeling on each dataset to see if there is any themetic pattern suggesting the relationship between race and lactose intolerance. I built six topics for each dataset. The topics generated from the lactose dataset are described below. 

The first topic is related to the symptoms of stomach 
<img width="629" alt="Screen Shot 2023-01-11 at 1 20 18 AM" src="https://user-images.githubusercontent.com/89910851/211742361-8c10a63a-9538-4331-8bd9-0e41ad2af68a.png">

The second topic is about lactase and enzyme. 

<img width="635" alt="Screen Shot 2023-01-11 at 1 21 05 AM" src="https://user-images.githubusercontent.com/89910851/211742523-51401d7a-425d-4bfc-b3f1-1ea1deb89a14.png">


