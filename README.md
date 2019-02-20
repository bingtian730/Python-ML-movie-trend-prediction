# movie-trend-prediction1
data analysis for a movie data from kaggle
Conclusions
Before any conclusion I noticed some data lmitations:

I dropped the rows with missing values and that might case bias for data analysis result.

The movie_data that collected were not evenly distributed,there are more than 12000 movie data from 2006-2015, about 6000 from 1996-2005, and about 4000 from 1986-1995, less than 2000 each from 1960-1985, which could also case data bias.

The mean of the popularity number is going up over time, which might case result favor to the movies that are more recent.

Conclusions: For question 1: There’s no correlation coefficient between revenue and runtime, month, year.(cc<0.2) There’s weak correlation coefficient between revenue and vote_average.(cc:0.2~0.4) There’s strong positive correlation coefficient between revenue and popularity, budget.(cc>0.6)

For question 2:

So for the whole dataset we have, from 1960-2015: The most popular genes are Adventure, Science Fiction( average popularity >1). The second most popular genres are Fantasy, Action, Animation,Family( 0.77<average popularity<1) The middle popular genres are Crime ,Thriller, War. ( 0.6<average popularity<0.77) The second least popular genres are Mystery, Comedy, Romance, Drama, Western, History, Music, Horror. ( 0.3<average popularity<0.6) The least popular genres are TV movie, Foreign, Documentary. ( average popularity<0.27)

But we have a lot more data from 2006-2015 and 1996-2005 then previous generation I plot histgram show in each decade how the gerens are distributed: 2006-2015 The most popular genres are adventure, science fiction, western, fantasy, action. 1996-2005 The most popular genres are fantasy, adventure, action, science fiction.animation. 1986-1995 The most popular genres are animation, adventure, fantasy, comedy, family. 1976-1985 The most popular genres are adventure, science fiction, action, family, fantasy. 1960-1975 The most popular genres are animation, adventure, family, crime, thriller.

And the proportions of genres for movies: From 2006-2015 The most genres of movies are drama, comedy, thriller, action. From 1996-2005 The most genres of movies are drama, comedy, thriller, action From 1986-1995 The most genres of movies are drama, comedy, action, thriller From 1976-1985 The most genres of movies are drama, comedy, action, thriller From 1960-1975 The most genres of movies are drama, comedy, action, thriller.

But this conclusion are based on the popularity number, which I mentioned on the previous data limitations, certain genres are more popular might because they're from the recent decade. From the bar chart, they showed that the more recent dacade had relavtively higher popularity score;The mean popularity is higher in the later decades for most of the genres.

So I decided to calculate the The relative genres popularity(RGP) change over time ( relative genres popularity= each genres average popularity/ average popularity of the decade)

Fantasy RGP from highest to lowest is1996-2005, then 2006-2015, then 1986-1995, Mystery RGP from highest to lowest is 1996-2005, 2006-2015, then 1986-1995, 1960-1975 then 1976-1985. Adventure RGP from highest to lowest is 2006-2015, 1976-1985, 1960-1975, 1996-2005, 1986-1995. Animation RGP from highest to lowest is 1986-1995, 1960-1975, 1996-2005, 2006-2015, 1976-1985. Science fiction RGP from highest to lowest is 2006-2015,1976-1985,1996-2005,1986-1995,1960-1975. Action RGP from highest to lowest is 2006-2015,1976-1985,1996-2005,1996-1995,1960-1975. Family RGP from highest to lowest is 1960-1975,1986-1995,1976-1985,2006-2015,1996-2005. Horror RGP from highest to lowest is 1996-2005,1976-1985,1986-1995,1960-1975,2006-2015. Thriller RGP from highest to lowest is 1960-1975,1986-1995,2006-2015,1996-2005,1976-1985. Drama RGP from highest to lowest is 1960-1975,1986-1995,1976-1985,2006-2015,1996-2005. Crime RGP from highest to lowest is 1986-1995,1960-1975,2006-2015,1996-2005,1976-1985. Comedy RGP from highest to lowest is 1960-1995, 1966-2005,2006-2015. Romance RGP from highest to lowest is 1986-1995,1996-2005,1960-1975,1976-1985,2006-2015.
