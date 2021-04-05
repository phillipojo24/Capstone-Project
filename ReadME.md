
# Intellgent Travel Recomendation System


**INTRODUCTION**

Everybody loves to travel or atleast dreams of it, but the fear of spending a gross amount of time sitting and planning a trip keeps us sitting on the couch and not out traveling the world. We must go through and budget every hotel, attraction, resturant and hope to find something similar to our likes that we want to do. The entire process is extremely tedious.

Pouplar travel tends that have been trending in the market are:

**Weekend Getaways:** This is for the short-term travelers which still want an authentic experience that are personal, rewarding and tailored to their interests.

**Bleisure Travel:** This is for the travelers that visit a location for business and extend it for liesure.

**Insta-Tourism:** This is for the travelers that want to formulate a trip on photogenic spot that are instagram worthy.

**Romantic Getaways:** This is for the travelers that what to grab there partner and hit the road to adventure.

**Goal:**
Our intellgent travel recomendations system will provide the user details and prefrencences on the most popular attractions in various loactions based on the type of travel class you fall under. This project will be the one-stop tool for travelers planning their vacations, we achive the same using Data Science tolls and techniques which will be explained in detail.

# What is a Recommendation System?

Machine learning algorithms in recommender systems typically fit into two categories: content-based systems and collaborative filtering systems. Modern recommender systems combine both approaches.

**Content-based methods** are based on the similarity of attributes. 

![image.png](https://raw.githubusercontent.com/phillipojo24/Capstone-Project/master/1_mz9tzP1LjPBhmiWXeHyQkQ.png)

**Collaborative filtering**, the system is based on past interactions between users and attractions. Ex: Ratings or Thumbs up Thumbs down. 

# Trip Recommender System Development

WebDriver drives a browser natively, as a user would, either locally or on a remote machine using the Selenium server, marks a leap forward in terms of browser automation. This tool was used to web scrap the diffrent attractions and differnt destination. I chose this route because if i wanted you use the traditional Beautiful Soup webscraping technique, i would have to genrate all the diffrent urls and it would have been time costly. 

For more information, access [link text](https://selenium-python.readthedocs.io/) 

## Movie Recomendation with KNN

KNN is a perfect go-to model for this use case and KNN is a very good baseline for recommender system development. 



![Collaborative filtering approach.PNG](https://raw.githubusercontent.com/phillipojo24/Capstone-Project/master/Screen%20Shot%202021-04-02%20at%2011.32.45%20AM.png)

**These are the recomendations generated from a collaborative filltering approach**

![Content based approach.PNG](https://raw.githubusercontent.com/phillipojo24/Capstone-Project/master/Screen%20Shot%202021-04-02%20at%2011.32.55%20AM.png)

These are the results genertated from a content-based approach.

# Conclusions

* The content based approached recommendation score was determined but the description of the different attractions. The collaborative approach was determined using the “user-label” rating of each attraction. Notice we have a higher scores vs when using the collaborative approach. Based on the content, has the model has captured that theses are similar attractions as percent match. 



* Since we were iterating through a list of cities the webdriver did perform the web scraping task quite slowly. Hopefully next time we can use a REST api to be able to call the data from the database much more quickly.





* Tf-idf Vectorizer versus the Countvectorizer had an impact on how the model performed in the end. Both suffered by the curse of dimensionality but they help to eliminate the cold start problem most recommendation systems run into. Countvectorizer performed better since it wasn't so detailed. 


# Future Work

1. Implement a hybrid recommender system and this hybrid recommender can offer both popular and less-know content to users.

2. There are several other website that can contain more relevant travel information on the items and hence can be be used for better predictions.

3. Model to also predict flight prices and "best" times to purchase a flight.

4. Eliminate under 18 recommendations and emphasize on suggesting kid friendly places.



```python

```
