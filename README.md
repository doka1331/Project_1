# Project_1
Group 2 Project 1 

FINALIZED SLIDE DECK: Project_1_Group_2_final.pptx

TYLER'S FILES:
  Project1_Script_Walje.ipynb,
  Project1_Written_Analysis_Walje.docx

MICHAEL'S FILES:
	CleaningScript.ipynb,
 	RegressionScript.ipynb,
  	Written_Analysis_final.docx

JADE'S FILES: 
	JadeAnalysis.ipynb
	

**TYLER'S ANALYSIS**
1.	Is there a relationship between IMDB Rating and the total amount of money earned by movies?
    a.	I believe this is an interesting question to examine because of the potential relationship between the two statistics. One might assume that the higher a movie is rated, the more money that movie will generate (and visa versa). If we do find a relationship (positive correlation) between IMDB Rating and the total amount of money earned, that would allow us to, in general, predict how well a movie performed in the Box Office solely based on that movie’s IMDB Rating.
2.	If we do not find any kind of correlation between IMDB Rating and the total amount of money earned, I will look at individual actors and see if that would provide a better idea of each of those statistics.
    a.	This will be an interesting follow-up, as many people associate high profile actors with great movies. We can once again use correlation as a measurement as to the strength of these relationships. More importantly, if we isolate some of those high profile actors we may see more of a correlation than we do with the entire data set. 

Findings:
	There was no meaningful correlation between IMDB Rating and the total amount of money earned. The exact calculation provided a correlation of 0.13, which is a very weak score for correlation. We would have needed to have seen a correlation above or around 0.8 for IMDB Rating and the total amount of money earned to have a strong enough relationship to provide any kind of predictive value.
	I completed this by calculating the correlation coefficient on Jupiter notebook and then plotting the results onto a scatter plot. This allowed me to observe the actual data as well as get the exact correlation results printed right on the plot.

	There was also no meaningful correlation between individual actors/directors and both IMDB Rating and the total amount of money earned. This means that we cannot predict how much money a movie will make or what the IMDB rating will be based on the actors in that movie. 
We also found that focusing on high profile actors only yielded a slightly higher correlation between IMDB Rating and Total Money Earned when compared to the overall data set.

Takeaways:
	Based on the findings from our current data set, it has proven difficult to find any predictive value or any meaningful positive correlation between the IMDB Rating and the total amount of money that movie has earned. This means that if we know exactly how much money a movie has made it will be difficult to predict what the IMDB Rating is, and if we know the IMDB Rating it will be difficult to predict how much money the movie has made.
	Concurrently, looking at individual high profile actors did not provide any more meaningful correlation or predictive value between the IMDB Rating and the total amount of money that movie has earned.
	Overall, there is no meaningful correlation between the IMDB Rating and the total amount of money that movie has earned. if the goal is to find predictive value in any of these statistics, more work is to be done.

Things to Improve:
-	With the parameters of this presentation there wasn’t enough time to do a real deep dive. For example, I only looked at Robert De Niro when looking at the correlation between IMDB Rating and the total money earned with a specific actor. There is certainly more to be discovered looking at other individual actors and directors.
-	This was a very clear dataset but it would certainly help to have access to other datasets and to build unique data frames based on those other datasets. That would provide us with more robust information and more ways to analyze this information.

**MICHAEL'S ANALYSIS**

Dong Woo (Michael) Kang
Steven Green
DU-VIRT-DATA-PT-12
Project 1 Written Analysis

Research Question
	The question for research that I inquired about was the relationship between the User IMDb rating and Critic-centered Meta-score for the IMDb Top 1000 movies. How do the two compare and if a relationship exists, what kind of relationship is it? 
 
Introduction
	First a little background, the IMDb is an online user-inputted internet movie database. In fact, the acronym IMDb stands for Internet Movie Database. It contains information related to everything film and cinema; and the information can be inputted by online users with very little restriction. The IMDb Top 1000 movies is a unique and specific dataset that contains the IMDb 1000 top-rated movies from over the years and information relating to each movie’s public receptance, including the two variables at study: User IMDb rating and Critic-Centered Meta-score. User IMDb rating is a score that is summarized out of a rating scale from 1-10 that registered IMDb users can rate a movie title/series out of. These scores are aggregated and then averaged out to represent the total IMDb rating of a select movie title/series. The Critic-centered Meta-score is a bit more difficult to understand; this is a numerical score that is calculated by a third-party company named Metacritic and is used by IMDb to show a more focused and concise rating by professional movie critics. Metacritic calculates Meta-Score by aggregating and averaging out a percentage score inputted by a sample population of incredibly respected movie and film critics. In order to be a part of this sample population of highly respected critics, Metacritic enacts a rigid code of expectation that critics must meet before being accepted into the sample. 
 
Data-Cleaning and Organizing
	Before conducting any cleaning, I imported my necessary Pandas libraries and commands into my Jupyter Notebook script. I then read in my raw data set that we obtained from Kaggle that was titled “imdb_top_1000.csv” with the necessary Pandas library commands. Following that I immediately removed columns: “Poster_link” and “Overview” as we agreed as a group that we did not need data containing movie summaries and online links to IMDb websites. After removing those selected columns, I dropped any rows of data that contained null values for any of the remaining columns and that brought our total rows of data to 714 total data inputs. Now that we had a cleaned set, I went on to rename columns to be more legible and coherent. It was also discussed as a group that numerical analyses will be taking place so I converted all numerical columns to float types so that analyses could be correctly conducted in Pandas, I further added Pandas formatting to these numerical columns to more clearly depict what each column represents. I copied this finalized data frame to a new CSV file and began conducting my analysis.
 
Data-Analysis: Results of User IMDb Rating VS Critic-centered Meta-score
	I began my research by comparing the average User IMDb Rating to the average Meta-Score of the entire dataset of IMDb top 1000 movies. I then wanted to know which values were given out the most for the dataset of IMDb top 1000 movies and so I retrieved the mode for both columns. What I found was that the average User IMDb Rating (7.937) and average Meta-Score (77.1582) were both slightly higher in value than the mode for each respective column; User IMDb Rating mode (7.7) and Meta-Score mode (76.0). I also found out that IMDb Users and Metacritic selected critics had a general approval rating of between 70%-80% for the top 1000 rated movies in the IMDb database. 
	I then wanted to see if this positive relationship of datapoints meant causation or correlation, in that, User IMDb Rating has a notable and significant impact on Critic-Centered Meta-Score. I first used a scatterplot and then I used a scatterplot with a calculated regression line to visualize this relationship. It is also important to note that because we are looking at IMDb’s top 1000 movies, no IMDb score or Meta-score was found to be below the IMDb rating value of 7 and Meta-score value of 25.  However, what I found was that while there is a positive relationship between User IMDb Rating and Metacritic’s Critic-centered Meta-score, there is little to no causation or correlation, in that, the variation in User IMDb Rating has little to no influence on the variation found in Metacritic’s Critic-centered Meta-score. If you look at the scatter plot without the regression line, one can see that the majority of datapoints are skewed to the upper left of the data set signifying that a majority of movies scored on the lower end by IMDb Users were actually scored relatively higher by Metacritic Critics. In addition, when analyzing the scatterplot with regression calculations, one can see that while a positive relationship exists, for each and every single unit increase in User IMDB Rating we see a corresponding 11.88 value increase in Meta-Critic Metascore for the entire dataset (slope value = 11.88), and the regression line depicted represents a positive relationship between the two scores, the calculated R-value (0.0789) signifies that only 7.89% of the variation in Metacritic’s Critic-centered Meta-score is caused or explained by the variation in User IMDb rating.

Conclusion
	 While it is easy to observe that User IMDB Rating and Metacritic Critic-centered Meta-score have a positive relationship, after further research, it is revealed that, in this case, a positive relationship does not indicate correlation or causation. While higher IMDB User Ratings usually do correspond with higher approval from Metacritic Critics, it is statistically proven that the Metacritic Critics do not take into account User IMDB Rating when calculating their own respective scores of a selected movie title or series. It is also good to note that because we are looking at the Top 1000 rated movies (and not some random movie data set sample) so the scores we are looking at and analyzing are on the high end of the spectrum. 

