# Twitter_Sentiment_Analysis
Use of Twitter API, Sentiment Analysis


## Interesting findings:
+ **'China' and 'India' dominated the keyword list!**
+ **Negative tweets are more likely related to sports?!**
+ **Public attention quickly drifted away from COVID-19 when Christmas comes!**


In this project, I demonstrate the use of Twitter API (V2) to download weekly tweets that contain the keyword "#covid19". The date is fixed from Dec. 18, 2022 to Dec. 25, 2022. Use of some preliminary text processing techniques (removing stopwords, lemmatization) as well as sentiment/subjectivity score calculattion will be demonstrated. In addition to that, some visualization are created in order to answer some questions of interets:

#### Questions of Interest:

**1. How popular is the keyword "#covid19" during the past week?**

**2. What are the proportion of positive, negative and neutral tweets that are related to #covid19?**

**3. What is the relationship between subjectivity score and sentiment score?**

**4. What are the contexts/themes of those positive, negative and neutral tweets? Do they differ?**

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

**4. What are the contexts/themes of those positive and negative tweets? Do they differ?**

#### Annotation of Negative Tweets
<img width="369" alt="image" src="https://user-images.githubusercontent.com/59629686/209506998-a4e914ec-88a4-40f2-83de-cf92af9d2d9a.png">


#### Annotation of Positive Tweets
<img width="423" alt="image" src="https://user-images.githubusercontent.com/59629686/209506970-e7b05486-1209-4e4c-a8f9-c3f951c97d46.png">


Note: The "annotation" labels are created by Twitter for the purpose of supporting some platform features, such as "Topic". We will use this as a reference and roughly get an idea of what those #covid19 conversations are about. In the above charts, annotations and their mean sentiment scores, frequencies and percentage with respect to all tweets are shown. Some findings are:

+ Both positive and negative tweets share some common, popular annotation tags, including "Ongoing News Story", "Events", "Person", "Business Taxonomy" abd "Politician".

+ Positive tweets are more often linked to "Interests and Hobbies", "Entities" and "Brand".

+ Negative tweets are more often linked to "Sports", "Sports League" and "Sports Team" and "Sport Event".


**5. What are the most popular/interesting keywords found in positive, negative and neutral tweets? What do they imply about the recent COVID-19 discourse on Twitter?**

#### All Tweets
![image](https://user-images.githubusercontent.com/59629686/209507589-25dada1c-7e6e-4acf-b47e-86ea4887a757.png)
<img width="644" alt="image" src="https://user-images.githubusercontent.com/59629686/209507631-32e7127b-06d5-467b-9e63-6ef17939d543.png">

#### Positive Tweets
![image](https://user-images.githubusercontent.com/59629686/209507657-4c387130-35ee-42fa-8c8b-10f3b6a2b668.png)
<img width="617" alt="image" src="https://user-images.githubusercontent.com/59629686/209507738-0ce137d3-926a-41ed-81c8-d3055e693f85.png">

#### Negative Tweets
![image](https://user-images.githubusercontent.com/59629686/209507772-e49ebd9c-b015-485d-ba09-1fa7e025b803.png)
<img width="617" alt="image" src="https://user-images.githubusercontent.com/59629686/209507804-e1b0b586-c1b5-4cc7-96d8-fe3d64303a55.png">

#### Neutral Tweets
![image](https://user-images.githubusercontent.com/59629686/209507821-ea168c1e-9c63-45ae-9cf9-6a6d9eedc652.png)
<img width="624" alt="image" src="https://user-images.githubusercontent.com/59629686/209507849-8cd3170e-5243-4277-82b5-fa9a0838dada.png">


Summary:
+ The top 5 keywords among all tweets are: China, India, Coronavirus, People, World
+ The top 5 keywords among positive tweets are: India, China, case, vaccine, like
+ The top 5 keywords among negative tweets are: China, World, Death, India, Coronavirus
+ The top 5 keywords among neutral tweets are: China, India, Coronavirus, new, vaccine

Finding: 
+ There seems no significant difference in terms of popular keywords for different sentiment categories. 
+ "China" and "India" are among the most popular words.
+ Some background knowledge: China recently had its biggest COVID outbreak since 2020 due to the cancellation of its zero-covid policy.
+ "Covid-is-not-over" appears as one of the top keywords in all 3 sentiment categories.
+ "Vaccine" appears often in neutral tweets, suggesting much less public sentiment towards mRNA vaccine as compared to before.
+ Among negative tweets, some popular words including lockdown, control, stupidity, fool.
+ Among positive tweets, some popular words including positive, mask, new, like


**6. How does the sentiment score fluctuate on an hourly basis during the past week?**

![ts1](https://user-images.githubusercontent.com/59629686/209509280-da6256d1-b430-42b8-885b-1782c32994f7.png)
![ts2](https://user-images.githubusercontent.com/59629686/209509291-22778401-9a8e-4458-9c86-6726051d4528.png)
![ts3](https://user-images.githubusercontent.com/59629686/209509296-a295fa40-a018-4704-8f1a-68c6610da935.png)

+ Overall, no obvious trend, nor any seasonality is detected based on the hourly time-series plot.


