COVID19 Twitter Sentiment Analysis - Visualization Dashboard using Node-RED on IBM Cloud
=========================================================================================

COVID-19 has wrecked havoc in all spheres of life, in every part of the world. One of the worst affected country is India. Government of India has initiated complete lockdown to maintain social distancing to curb the growth of the virus. Citizens have a mixed feeling towards this lockdown, and the outrage has been evident on social media ( Facebook, Twitter) . 
       In this project we aim to analyse the sentiments of the people through Twitter hashtags (#), to identify whether the opinion expressed by the individual is positive or negative and will try to build a predictive analytics model to understand the behavior of people if the lockdown is further extended.
       
We have used Node-RED application from IBM Cloud Services to create our app. We have 6 main nodes :- 

a) Twitter Node ( which pulls in tweets in realtime from a twitter account and forwards them as payload ) 

b) Sentiment Node ( which assigns a sentiment score to the payload . It is a Node-RED node that scores incoming words using the AFINN-165 wordlist and attaches a sentiment.score                       property to the msg ) 

c) Join Node ( which joins the sentiment scores to form a value within a specific time interval . We gave a time interval of 10 secodns . It combines arriving from different sources into a single message ) 

d) Function Node ( which calculates the average sentiment score of the messgaes over the 10 seconds time interval )

e) Chart UI Node ( which displays the average sentiment score over a linear chart ) 

f) Gauge UI Node ( which displays the average sentiment score over a gauge chart ) 

App URL
https://twitter-sentiment-analysis-of-covid19-hashtags.eu-gb.mybluemix.net/ui 
