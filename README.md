# Twitter_Sentiment_Analysis
Use of Twitter API, Sentiment Analysis



In this project, I demonstrate the use of Twitter API (V2) to download weekly tweets that contain the keyword "#covid19". The date is fixed from Dec. 18, 2022 to Dec. 25, 2022. Use of some preliminary text processing techniques (removing stopwords, lemmatization) as well as sentiment/subjectivity score calculattion will be demonstrated. In addition to that, some visualization are created in order to answer the following questions:

#### Questions of Interest:

**1. How popular is the keyword "#covid19" during the past week?**

**2. What are the proportion of positive, negative and neutral tweets that are related to #covid19?**

**3. What is the relationship between subjectivity score and sentiment score?**

**4. What are the contexts/themes of those positive, negative and neutral tweets?**

**5. What are the most common/interesting keywords found in positive, negative and neutral tweets? What do they imply about the recent COVID-19 discourse on Twitter?**

**6. How does the sentiment score fluctuate on an hourly basis during the past week?**



## Plots

**1. How popular is the keyword "#covid19" during the past week?**

![image](https://user-images.githubusercontent.com/59629686/209488792-ed4fd37b-41b9-4bb8-9f16-a24386783b8d.png)

+ There is an obvious trend here: the number of tweets related to #covid19 increased from December 18, 2022 to December 21, 2022, and started to decline since then. One possible explanation is that, as it gets closer to the Christmas (Dec 25) and since there isn't any major outbreak domestic-wise (we will latter see that recent tweets on #covid19 are mostly related to 'China' and 'India'), people care less about #covid19.

**2. What are the proportion of positive, negative and neutral tweets that are related to #covid19?**

![pie](https://user-images.githubusercontent.com/59629686/209498657-fab0b4bd-8206-4309-bf41-44874fcf0047.png)

+ The plot above shows the relationship between subjectivity score and sentiment score (attitude). Neutral tweets tend to have lower subjectivity score; negative and positive tweets have very similar distribution in terms of subjectivity score. 

**3. What is the relationship between subjectivity score and sentiment score?**

![box](https://user-images.githubusercontent.com/59629686/209498716-72dcb9b6-6e96-416f-b1ef-0fc8a1ded27e.png)

+ We may also look at the relationship between subjectivity score and sentiment score category. The plot above shows that neutral tweets tend to have lower subjectivity score; negative and positive tweets have very similar distribution in terms of subjectivity score. It makes sense as neutral comments tend to be less subjective. 

**4. What are the contexts/themes of those positive, negative and neutral tweets?**

#### Annotation of Negative Tweets
<img width="375" alt="image" src="https://user-images.githubusercontent.com/59629686/209498862-4202bf8a-bf3b-471d-8282-c426ae8e3ddc.png">


#### Annotation of Positive Tweets
<img width="373" alt="image" src="https://user-images.githubusercontent.com/59629686/209499070-79fb5804-d627-499f-aa16-7238bf77ebe3.png">


