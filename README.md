# MA-Thesis

`Reddit_data.ipynb` is a notebook for scraping Reddit data from the following subreddits **lactoseintolerant** , **lactoseintolerance** , **milkmemes** , **AncestryDNA** , **23AndMe** , **MyHeritage**. All posts and comments are scraped from each subreddits. For the first three subreddits, the posts are combined into a dataframe and the comments are combined into a dataframe, which I named as **lactose_df_posts** and **lactose_df_comments** because these three subreddits are related to lactose. The other three subreddits are combined into another dataframe (posts and comments separated), named as **genome_df_posts** and **genome_df_comments** for they are related to genetics. After some data cleaning, there are 6,992 posts and 41,813 comments in the lactose dataframe; 25,852 posts and 768,767 comments in the genome dataframe. 

`Exploratory Analysis.ipynb` is a notebook for exploring the datasets. I am going to analyze the lactose_df and the genome_df separately. First of all, I would like to count the number of words related to 'race' and 'genes' appearing in the lactose_dfs. On the other hand, I would like to count the number of words related to 'lactose' appearing in the genome_dfs. I did the word count, as well as identify the original posts/comments that the word appear (exported into csv for further interpretation). It turns out that a significant number of race-related/genetic-related words ( 707 times) appear in the lactose_dfs and the same happend to lactose-related words (492 times) in the genome_dfs. This finding suggests that lactose and genetics are closely associated in these subreddit discourses. 
Next, I ran LDA topic modeling on each dataset to see if there is any themetic pattern suggesting the relationship between race and lactose intolerance. I built six topics for each dataset. The topics generated from the lactose dataset are described below. 

The first topic is related to the symptoms of stomach 
<img width="629" alt="Screen Shot 2023-01-11 at 1 20 18 AM" src="https://user-images.githubusercontent.com/89910851/211742361-8c10a63a-9538-4331-8bd9-0e41ad2af68a.png">

The second topic is about lactase and enzyme. 

<img width="635" alt="Screen Shot 2023-01-11 at 1 21 05 AM" src="https://user-images.githubusercontent.com/89910851/211742523-51401d7a-425d-4bfc-b3f1-1ea1deb89a14.png">

The third topic is related to very specific food that causes lactose intolerance such as yogurt, cream cheese. 
<img width="598" alt="Screen Shot 2023-01-11 at 1 22 02 AM" src="https://user-images.githubusercontent.com/89910851/211742701-a5e7df08-00fa-40f9-9803-03a093f507a9.png">

The sixth topic is talking about the ingredients of food, such as protein, powder, sugar, cream. 
<img width="643" alt="Screen Shot 2023-01-11 at 1 23 30 AM" src="https://user-images.githubusercontent.com/89910851/211742957-79276bab-8dde-4c88-9b8e-c7fdba829ade.png">

It is hard to define the fourth and fifth topic. 

In a word, there is no topic directly talking about genetics and race. 

**for the genome dataset**, the first topic is related to human ancient history such as hunt-gatherer, competitor and great-grandfather.

<img width="671" alt="Screen Shot 2023-01-12 at 11 28 21 AM" src="https://user-images.githubusercontent.com/89910851/212138354-54da6b6f-b925-4e7e-be80-3e6c4c1f5791.png">

the second topic is about colonist, bavarian and germanic. 

<img width="669" alt="Screen Shot 2023-01-12 at 11 36 07 AM" src="https://user-images.githubusercontent.com/89910851/212138932-d17624a7-597c-4a95-840c-781084a7effe.png">

the third topic seems to be talking about southern plantation, Creole and slave 

In a word, there does not exist a topic explicitly or implicitly describes lactose intolerance or food. 
