# Grace Yang data science portfolio examples (THEME LEAP DAY)
Example data science portfolio


## [Project 1: High-Dimensional Embeddings of 60,000 Dating Essays](https://github.com/PlayingNumbers/ds_salary_proj)
* High-dimensional embedding using Google's Universal Sentence Encoder (USE)
* 2-dimensional cluster visualization using t-Distributed Stochastic Neighbor Embedding (t-SNE)
* I started with using Google's Natural Language Processing (NLP) embedding algorithms model, Universal Sentence Encoder, to produce 512 embedding dimensions for each dating essay.
* One of the ways of trying to visualize high-dimensional data is a tool called t-distributed Stochastic Neighbor Embedding or t-SNE. With t-SNE, we can look at the embeddings in two or three dimensional space. This is useful for checking if clusters existed in the data. For example, this is most famously observed in the example of passing through the MNIST data set of handwritten digits 0 to 9 and seeing 10 clusters quite clearly.
* I explored essay lengths ranging from 30 (roughly the first four to five words in an essay), to 70 (first sentence, or the length of good ”tweets” that were liked and most often retweeted on the Twitter app), and to 140 (first two sentences, or the character count limit for Twitter up through late-2017)
* Visualizations by age group, gender, pet preferences did not reveal any clear and separate clusters


## [Project 2: Approximate Nearest Neighbors (ANN) of 60,000 Dating Essays](https://github.com/PlayingNumbers/ds_salary_proj)
* I used Approximate Nearest Neighbors (ANN) to help filter/rank search algorithms and dating app user match recommendations
* For popular dating apps and websites like Tinder, Bumble, Match and OKCupid, their customer base ranges between two to eight million people. Match recommendations are not done with brute computation force across all possible pairings or combinations.
* Instead a common technique used that makes embedding comparisons more efficient is Approximate Nearest Neighbors (ANN). Given a customer’s self-summary essay or ”subject essay” and the position of its embedding in the high-dimensional space, ANN will search for other essay whose embeddings are mapped closer to this subject essay.


## [Project 3: Support Vector Clustering and Classification of 60,000 Dating Essays](https://github.com/PlayingNumbers/ds_salary_proj)
* I used Support Vector Machine (SVM) clustering to identify classifications in the dating essays.
* We applied the SVC classification tool to the 512-dimensional embeddings generated from Google’s Universal Sentence Encoder module. The classification heat maps and accuracy metrics indicated that there appeared to be something within the embeddings that was predictive of the gender of the dating app user who wrote the essay.
* Similar explorations by age group did not show classifications of good accuracies other than for those in their 20s.


## [Project 4: Sentiment Analysis of 60,000 Dating Essays](https://github.com/PlayingNumbers/ds_salary_proj)
* Sentiment Analysis


## [Project 5: Online Screen Time and Teen Mental Health](https://github.com/PlayingNumbers/ds_salary_proj)
* Causal inference study using largest survey on 20,000 households in the U.K.


## [Project 6: Regression Analysis on Heart Attack Patients](https://github.com/PlayingNumbers/ds_salary_proj)
* regression, etc.


## [Project 7: Time Series Study of Shark Attacks in the Last Century](https://github.com/PlayingNumbers/ds_salary_proj)
* time series, etc.




# [Ken's Example Project 1: Data Science Salary Estimator](https://github.com/PlayingNumbers/ds_salary_proj) 
* Created a tool that estimates data science salaries (MAE ~ $ 11K) to help data scientists negotiate their income when they get a job.
* Scraped over 1000 job descriptions from glassdoor using python and selenium
* Engineered features from the text of each job description to quantify the value companies put on python, excel, aws, and spark. 
* Optimized Linear, Lasso, and Random Forest Regressors using GridsearchCV to reach the best model. 
* Built a client facing API using flask 

##![](/images/positions_by_state.png)


# [Ken's Example Project 2: Ball Image Classifier](https://github.com/PlayingNumbers/ball_image_classifier) 
For this example project I built a ball classifier to identify balls from different sports. This could be useful for someone who is new to sports from a certain country. They could take a picture of a ball and an app could serve them some information about the history and rules of the game. This is the underlying model for building something with those capabilities. 

I was able to get the model to predict the sport of the ball with 94% accuracy after minimal tuning. For most of the cases this would meet the need of an end user of the app. To get these results I used transfer learning on a CNN trained on resnet34. This created time efficiencies and solid results. 

##![](/images/matrix_results.png)
