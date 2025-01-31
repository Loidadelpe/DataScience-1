# Project Design Writeup and Approval Template

Follow this as a guide to completing the project design writeup. The questions for each section are merely there to suggest what the baseline should cover; be sure to use detail as it will make the project much easier to approach as the class moves on.

### Project Problem and Hypothesis
* What's the project about? What problem are you solving?

The project is about predicting the best type of movie recommendation based on your taste for the MovieLens 1M dataset. The dataset contain 1,000,209 anonymous ratings of approximately 3,900 movies made by 6,040 MovieLens users who joined MovieLens in 2000.

I wil try to answer the question “What movie should I watch this evening?” The need to build robust movie recommendation systems is extremely important given the huge demand for personalized content of modern consumers.

Recommendation systems are used not only for movies, but on multiple other products and services like Amazon (Books, Items), Pandora/Spotify (Music), Google (News, Search), YouTube (Videos) etc.

My hypothesis is that the most meaningful our movie recommendation is the higher will be the engagement of our movie website (e.g. Netflix)


* Where does this seem to reside as a machine learning problem? Are you predicting some continuous number, or predicting a binary value?

Deep Learning / Neural Network as detail in this repo:

https://github.com/khanhnamle1994/movielens/blob/master/README.md
http://nbviewer.jupyter.org/github/khanhnamle1994/movielens/blob/master/Deep_Learning_Model.ipynb

I hope to attempt a simple deep learning approach to build a recommendation engine for the MovieLens 1M dataset. This model performed better than all the approaches attempted before (content-based, user-item similarity collaborative filtering, SVD). 

I believe I will be predicting a continuous number (rating) but I am unsure at this point as we haven't explored Neural networks yet.




* What kind of impact do you think it could have?

Recommendation Engine is your advisor to help you make the right choices by providing you tailored options and creating a personalized experience for you. It is beyond any doubt that recommendation engines are getting popular and critical in the new age of things. It is going to be in our best interest to learn to use them for businesses to be more competitive and consumers to be more efficient.

* What do you think will have the most impact in predicting the value you are interested in solving for?

I expect ratings, tags and genres to have the highest impact.



### Datasets
* Description of data set available, at the field level (see table)

The dataset that I’m working with is MovieLens, one of the most common datasets that is available on the internet for building a Recommender System. The version of the dataset that I’m working with (1M) contains 1,000,209 anonymous ratings of approximately 3,900 movies made by 6,040 MovieLens users who joined MovieLens in 2000.

RATINGS FILE DESCRIPTION
All ratings are contained in the file "ratings.dat" and are in the
following format:


UserID::MovieID::Rating::Timestamp

- UserIDs range between 1 and 6040 
- MovieIDs range between 1 and 3952
- Ratings are made on a 5-star scale (whole-star ratings only)
- Timestamp is represented in seconds since the epoch as returned by time(2)
- Each user has at least 20 rating


USERS FILE DESCRIPTION
================================================================================

User information is in the file "users.dat" and is in the following
format:

UserID::Gender::Age::Occupation::Zip-code

All demographic information is provided voluntarily by the users and is
not checked for accuracy.  Only users who have provided some demographic
information are included in this data set.

- Gender is denoted by a "M" for male and "F" for female
- Age is chosen from the following ranges:

	*  1:  "Under 18"
	* 18:  "18-24"
	* 25:  "25-34"
	* 35:  "35-44"
	* 45:  "45-49"
	* 50:  "50-55"
	* 56:  "56+"

- Occupation is chosen from the following choices:

	*  0:  "other" or not specified
	*  1:  "academic/educator"
	*  2:  "artist"
	*  3:  "clerical/admin"
	*  4:  "college/grad student"
	*  5:  "customer service"
	*  6:  "doctor/health care"
	*  7:  "executive/managerial"
	*  8:  "farmer"
	*  9:  "homemaker"
	* 10:  "K-12 student"
	* 11:  "lawyer"
	* 12:  "programmer"
	* 13:  "retired"
	* 14:  "sales/marketing"
	* 15:  "scientist"
	* 16:  "self-employed"
	* 17:  "technician/engineer"
	* 18:  "tradesman/craftsman"
	* 19:  "unemployed"
	* 20:  "writer"

MOVIES FILE DESCRIPTION
================================================================================

Movie information is in the file "movies.dat" and is in the following
format:

MovieID::Title::Genres

- Titles are identical to titles provided by the IMDB (including
year of release)
- Genres are pipe-separated and are selected from the following genres:

	* Action
	* Adventure
	* Animation
	* Children's
	* Comedy
	* Crime
	* Documentary
	* Drama
	* Fantasy
	* Film-Noir
	* Horror
	* Musical
	* Mystery
	* Romance
	* Sci-Fi
	* Thriller
	* War
	* Western

- Some MovieIDs do not correspond to a movie due to accidental duplicate
entries and/or test entries
- Movies are mostly entered by hand, so errors and inconsistencies may exist




* If from an API, include a sample return (this is usually included in API documentation!) (if doing this in markdown, use the javacription code tag)
N/A

### Domain knowledge
* What experience do you already have around this area?
I do have data analysis and market research experience but I will need to make myself familiar with the dataset and understand deep learning methodology as per our course programme and the blog stated above.


* Does it relate or help inform the project in any way?
Yes, hopefully my professional background helps backing up this project.


* What other research efforts exist?
    * Use a quick Google search to see what approaches others have made, or talk with your colleagues if it is work related about previous attempts at similar problems.
    * This could even just be something like "the marketing team put together a forecast in excel that doesn't do well."
    * Include a benchmark, how other models have performed, even if you are unsure what the metric means.
    
This blog states in detail the need for a recommendation engine and the 4 approaches considered:
 
https://medium.com/@james_aka_yale/the-4-recommendation-engines-that-can-predict-your-movie-tastes-bbec857b8223
    
The code for the 4 methodologies is saved here:
 
https://github.com/khanhnamle1994/movielens/blob/master/README.md

Here are the different notebooks:

Data Processing: Loading and processing the users, movies, and ratings data to prepare them for input into my models.

Content-Based and Collaborative Filtering: Using the Content-Based and Collaborative Filtering approach

SVD Model: Using the SVD approach

Deep Learning Model: Using the Deep Learning approach
    

### Project Concerns
* What questions do you have about your project? What are you not sure you quite yet understand? 
(The more honest you are about this, the easier your instructors can help).

I am also not 100% sure if what I will be trying to determine is the rating and how that links to a better movie recommendation at the end as my original dataset is not available anymore and I am not fully aware with what ca we achieved with the current.
I am not sure about where should I cut my dataset to make it work with the project restrictions (e.g. processing time for modelling)
I am also not sure about the steps I should follow after exploratory analysis as we haven't explored yet Neural Networks 
and finally, I am unsure about Neural Networks being the most appropiate methodology to apply considering that 4 methodologies outlined and the fact that we will be exploring it at the very end of the course

* What are the assumptions and caveats to the problem?

I asume the data is somehow appropiate and includes the variables needed for this analysis. However, I expect some degree of manipulation to be needed as usual. 

A caveat to consider is that my dataset is originally pretty big and in terms of ensuring our model to run in time I expect to need to reduce the number of observations. I am unsure about how many observations are ideal for analysis purposes while ensure high performance when running our model.

    * What data do you not have access to but wish you had?
I wish I could have more demographic information on users and geospatial could have been interesting.

    * What is already implied about the observations in your data set? For example, if your primary data set is twitter data, it may not be representative of the whole sample (say, predicting who would win an election)
My dataset only considers those users that provided demographic information. Therefore their profile might not be representative of the population's demographic profile as this information wasn't compulsory.
    
    
* What are the risks to the project?
    * What's the cost of your model being wrong? (What's the benefit of your model being right?)
 If our model is wrongly applied to our website, we risk lowering our customer engagement metrics due to incorrect movie recommendations.
 If our model is right, we expect incresing conversion rates and engagement with our services.
 
    * Is any of the data incorrect? Could it be incorrect?
    
 Yes, our data can be incorrect due to human errors. We are aware that some MovieIDs do not correspond to a movie due to accidental duplicate entries and/or test entries, movies are mostly entered by hand, so errors and inconsistencies may exist and demographic information has been provided by the end user freely so expect some degree of inconsistencies (typos, etc..)
 
 
### Outcomes
* What do you expect the output to look like?

I expect making a movie recommendation list of unrated 20 movies sorted by prediction value for a specific userId that is meaningful.

Something as good or even better than the last top 20 recommendation list stated on this notebook:

https://github.com/khanhnamle1994/movielens/blob/master/Deep_Learning_Model.ipynb


* What does your target audience expect the output to look like?

As per above notebook top 20 recommendation list

* What gain do you expect from your most important feature on its own?

I would consider this project a success if I was able to replicate and improve the engine recommendation made by James Lee as stated on his blog post:
https://medium.com/@james_aka_yale/the-4-recommendation-engines-that-can-predict-your-movie-tastes-bbec857b8223


* How complicated does your model have to be?

Ideally my model should be as easy as possible to ensure valid results

* How successful does your project have to be in order to be considered a "success"?

I would define success as obtaining a meaninful recommendation on movies with the given dataset. A big success would be improving the model already implemented by James Lee.

* What will you do if the project is a bust (this happens! but it shouldn't here)?
I will explore the reasons why the project failed and rebuild a new approach from there. Sure not everything is a failure so I would keep what works and work on what didn't to achieve the end goal.

