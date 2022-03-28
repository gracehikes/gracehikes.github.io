# Grace Yang data science portfolio examples (THEME SLATE)
Example data science portfolio


## [Project 1: High-Dimensional Embeddings of 60,000 Dating Essays](https://github.com/PlayingNumbers/ds_salary_proj)
* I first applied Google's Universal Sentence Encoder, a Natural Language Processing (NLP) embedding algorithms model, to get 512 embedding dimensions for each dating essay.
* One of the ways to visualize such high-dimensional data is t-distributed Stochastic Neighbor Embedding (t-SNE). With t-SNE, we can condense the high-dimensional embeddings in 2- or 3-D space. This is useful for visually checking if clusters existed in the data. One of the most famous examples of this applies t-SNE to the high-dimensional embeddings from the MNIST data set of handwritten digits 0 to 9 and seeing ten distinct clusters quite clearly.
* I explored embeddings from various essay lengths: 30 characters (roughly the first four to five words in an essay), 70 characters (first sentence, or the length of good ”tweets” that were liked and most often retweeted on the Twitter app), and 140 characters (first two sentences, or the character count limit for Twitter up through late-2017). I performed t-SNE visualizations by age group, gender, pet preferences to check for clear and separate clusters.


## [Project 2: Approximate Nearest Neighbors (ANN) of 60,000 Dating Essays](https://github.com/PlayingNumbers/ds_salary_proj)
* For popular dating apps and websites like Tinder, Bumble, Match and OKCupid, their customer base ranges between two to eight million people. Match recommendations are not done with brute computation force across all possible pairings or combinations.
* I used Approximate Nearest Neighbors (ANN) to help filter/rank search algorithms and dating app user match recommendations. Given a customer’s self-summary essay or ”subject essay” and the position of its embedding in the high-dimensional space, ANN will search for other essay whose embeddings are mapped closer to this subject essay.


## [Project 3: Support Vector Clustering and Classification of 60,000 Dating Essays](https://github.com/PlayingNumbers/ds_salary_proj)
* I used Support Vector Machine (SVM) clustering tool to identify classifications in the dating essays' 512-dimensional embeddings generated from Google’s Universal Sentence Encoder module. Text analyses on what people write in their dating profile self-summaries may help uncover similarities or differences for different features like gender, age group, socio-economic status, etc.
* The classification heat maps and accuracy metrics indicated that the embeddings were somewhat predictive of the gender of the dating app user who wrote the essay. Gender prediction accuracy of 65%. Similar explorations by age group did not show classifications of good accuracies other than for those in their 20s.


## [Project 4: Online Screen Time and Teen Mental Health](https://github.com/gracehikes/proj_social_media_teen_mental_health)
* Causal inference study using a 2019 survey on 20,000 households in the U.K. The teens were asked about their feelings regarding school work, appearance, family, friends, school and life as a whole. The response section showed a panel of different emoticon faces, where '1' is completely happy with a big smile to '7' which is not at all happy with a big frown. 
* There appeared to be adverse effects on a young person’s mental well-being when they spent in excess of 4 hours on social media chatting and interactions during a normal school day. The analysis of responses for six mental well-being questions from the U.K. 2019 data, when compared for different amounts of time that the young people spent on social media, produced such indications. While the effect estimates varied in magnitude, they were all directionally toward the more unhappy end of the scale for the six questions.


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
