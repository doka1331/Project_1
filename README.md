# Project_1
Group 2 Project 1 
TYLER'S FILES:
  Project1_Script_Walje.ipynb
  Project1_Written_Analysis_Walje.docx

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
