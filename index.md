## What image of Trump emerges from news articles between 2015 and 2020?

# Abstract

In 2016, the world was completely astonished: Donald Trump was elected president of the United States while all the polls estimated that Hillary Clinton would win. The following four years were marked by shocking declarations on Twitter, controversies, and withdrawals from previous agreements. But even though this president has been highly criticized by part of the international community, he was almost ready to run for a second term in 2020. So looking at quotes from this president as well as quotes about him might offer another perspective on this situation. This opens the door to many questions: What are the issues that Trump has addressed during his campaign and his presidency? How is he perceived by different segments of the population? Is there any influence from newspapers? Let's find out through a corpus of thousands of quotations related to Trump and extracted from thousands of English news articles published between 2008 and 2020.


# Introduction

Three main questions guided this study.

About Trump's program:
-  Which topics did Donald Trump talk about the most during the presidential campaign (starting in 2015), and during his time in office (20/01/2017 - 20/01/2021)? Indeed, before looking at what Trump's supporters (or detractors) thought of him, we need to understand what he had to offer to US citizens. But studying his official agenda is not satisfactory, as it is subjective and instrumented to cater to voters' expectations, and thus not representative of the candidate's true thoughts. On the other hand, we believe that looking for topics appearing in Trump's quotes over time can be more telling. Then, the aim was to look for change over time in the topics discussed, for example before and after his election, or because of external events such as the Covid crisis.

About Trump's supporters and opponents:
- Can we quantify Trump's popularity over time or according to the population group? So first the idea is to look at the sentiment of the quotes to quantify this popularity over time and and try to link it to current events. Secondly, it is interesting to look at whether this popularity depends on different population groups.
- In which newspapers are Trump's quotations published? One of the key events of the 2016 campaign was the massive use of both fake news by Russia to discredit Hillary Clinton and tweets to be present on social media. This campaign appears to be a mediatic battle, in which newspapers played a great role. Different information could be provided by this study, as the relation between political affiliation of a newspaper and the positivity of the quotes it published.

# Dataset
 
To answer the questions, we needed data. This took the form of quotations extracted from news articles in _Quotebank: A Corpus of Quotations from a Decade of News_ (TODO mettre une référence un peu plus propre ?). Briefly, this dataset is made of quotations that were extracted from English language articles, and their authors were estimated by the program with a confidence value. As the quotation corpus is huge (178 million quotations), we select only the quotations in the period which should a priori concern Trump the most, i.e. data from 2015 to 2020 (one year before Trump’s election until the end of his term). Furthermore, only the remaining quotations from Trump or talking about Trump in English were kept. After this preprocessing step, only 1,097,729 quotes remained, which is enough for our analysis, yet remains manageable.

# Results

## The evolution of Trump's speaking topics

Moreso than any other president, Trump liked to publish his thoughts on Twitter. Those then get quoted by news sites. For that reason, many of his ideas are available in our dataset. To extract them, we thus consider only the quotations spoken by Trump. At this point, the operation became a bit more complicated: how to determine the topics in Trump's quotations? We decided to use Empath, which is a tool for analyzing text across lexical categories. The text was classified using many topics, of which we retained the five which gave the most interesting results: Racism, Economy, Environment, Foreign policy, and Pandemic.

Below are shown word clouds for each topic, to illustrate what kind of vocabulary Trump uses to talk about the topics. In these, larger words were uttered more frequently.

<p align="center">
  <img src="https://user-images.githubusercontent.com/57459514/146549269-b955f224-9e15-4dcb-a8e3-b7dab6c187c4.png" width="400" />
  <img src="https://user-images.githubusercontent.com/57459514/146549292-d25f50b4-7573-451b-b719-fbb39f406585.png" width="400" />
  <img src="https://user-images.githubusercontent.com/57459514/146549309-c24c80b3-4ade-44be-b548-d008372c0b4b.png" width="400" />
  <img src="https://user-images.githubusercontent.com/57459514/146549313-60849da0-de3c-41f7-9eb6-00fc555a8423.png" width="400" />
  <img src="https://user-images.githubusercontent.com/57459514/146549316-7e4c84f4-f1a7-4aa8-93a6-96e7243ec8f7.png" width="400" />
</p>

First off is the graph for the Racism topic. We can see that the topic is much more actively discussed by Trump before than during his time in office. The 2015 peak might be interpretable as linked to the death of Freddie Gray, on which Trump commented.
<p align="center">
  <img src="https://user-images.githubusercontent.com/57459514/146547879-3e12cce3-c8eb-45a5-9e60-232251e9dab0.png" width="1400" />
</p>
The Economy topic is much more present before the election, which makes sense as Trump spent the whole campaign claiming that China was hurting the American economy by devaluating the yuan.
<p align="center">
  <img src="https://user-images.githubusercontent.com/57459514/146547894-e8b5029c-15ed-4353-8828-2bf52a1aaa86.png" width="1400" />
</p>
Below is shown the Environment topic, for which the three maxima also occur before or right after Trump entered office, but not much talk afterwards. This is understandable as Trump favored acting in the shadows for this topic, having discretely suppressed 68 laws on environment.
<p align="center">
  <img src="https://user-images.githubusercontent.com/57459514/146547906-80e30c6d-b5ca-41a0-b799-ce56ebc9dbad.png" width="1400" />
</p>
Next up is the Foreign Policy, a topic which Trump relatively ignored before he was elected, but then took great importance. Indeed, during his time in office, Trump faced several foreign crises. We interpret the three major peaks on the graph as follows:

 - 2017 peak: this probably corresponds to the crisis with North Korea (this is supported by the prominence of "Korea" in the word cloud). 
 - 2018 peak: could be linked to the crisis with Pakistan ("Pakistan" and "Afghanistan" are important words in the word cloud), as Trump tweeted in January that Pakistan rewarded US aid with "nothing but lies and deceit".
 - 2019 peak: could correspond to the Ukraine affair, in which, in September 2019, a whistleblower revealed that Trump asked the Ukrainian president to investigate Joe Biden's son.
<p align="center">
  <img src="https://user-images.githubusercontent.com/57459514/146547915-45294a37-9a04-4371-bfa9-2bb08fb61a9d.png" width="1400" />
</p>
The last topic we selected is Pandemic, with a sharp increase at the beginning of the Covid-19 pandemic, and almost no prior discussion.
<p align="center">
  <img src="https://user-images.githubusercontent.com/57459514/146547862-e5ff3cea-5fc5-4af8-88c4-5217b3d067c7.png" width="1400" />
</p>
Finally, we show the evolution of the topics all together. We notice that the scales of topic frequencies are quite different, with Economy and Environment being relatively less frequent and Foreign policy (and eventually Pandemic) being more prominent in Trump's speech. 
<p align="center">
  <img src="https://user-images.githubusercontent.com/57459514/146547835-350d8e20-cf47-4ddc-8e15-1255e948d8ca.png" width="1400" />
</p>

## Trump's popularity

### Trump's popularity in the population

During all his political involvement, Trump was described as a divisive figure. The controversies he created reinforced the adhesion of a part of the population, and reinforced the opposition of the other part. But is this trend visible in quotes from people talking about Trump? We applied the Vader sentiment analysis model on the quotes talking about Trump, i.e. quotes that include the word "Trump" except those authored by Trump. This method allows us to determine the degree of positivity. This sentiment is given by a number, called the compound, between -1 and 1. The closer to 1, the more positive the quotation, the closer to -1, the more negative. 

First, we look at the sentiments of the quote set over time.

<p align="center">
 <img src="https://user-images.githubusercontent.com/91223105/146583542-64ca0983-592f-4b22-8095-f1502640f4b5.png" width="1000" /> 
</p>

One of the first trends we see while looking at this graph is that the peaks are strongly correlated with a small number of quotes for this period of time. To reduce the variance, we decided to group the quotes on a 6 month time window instead of only one month.

<p align="center">
 <img src="https://user-images.githubusercontent.com/92359177/146580435-dca42bd7-18bd-4f57-a343-e44278e9c554.png" width="700" />
</p>
 
This is quite better, the fluctuations are not correlated with the number of quotes anymore! To be sure that our result is in accordance with the reality, we compared our results with a <a href="https://projects.fivethirtyeight.com/trump-approval-ratings/">graph of Trump's popularity rating over time</a>. Overall, the trend seems quite similar with what we have.

Plotting over months can hide general trends over years.

<p align="center">
 <img src="https://user-images.githubusercontent.com/92359177/146580564-907fa3be-6400-477a-8b0e-9c25be0b0c27.png" width="400" />
</p>

It appears that Trump's popularity decreased from 0.22 to 0.15 between 2015 and 2019, meaning a 7% decrease in 4 years. Between 2019 and 2020, his popularity increased to reach 0.19, but this is probably due to the decrease in quotations about Trump, leading to a huge variance in the result (almost 10% against 4% in 2018). As a conclusion, the more time Trump passed in office, the lower his popularity rating.

But is this trend representative of all the American population? Probably not. So to distinguish people that agree or not with Trump policies, we used information provided about the speakers.

We plotted the mean compound value for several speaker parameters. The numbers on the graphs correspond to the numbers of quotations for each label.

<p align="center">
 <img src="https://user-images.githubusercontent.com/92359177/146584161-ffc6058b-ab07-4c46-9933-8b94b5bd9529.png" width="300" />
</p>

For nationality, countries in Europe, Australia, and North America are more supportive of Trump than those in Africa and Asia. We can see in particular that the South America continent is largely under-represented compared to the others. Africa is also under-represented but in a less marked way.

<p align="center">
 <img src="https://user-images.githubusercontent.com/92359177/146584244-b813524f-3a27-4d13-b482-d761cc8ff1b8.png" width="300" />
</p>

For gender, it is males who are more supportive of Trump than females. It appears that more men are quoting when talking about Trump than women (7979 against 1747), however these differences in numbers are probably due to biases in the original database rather than the subject of Trump.

<p align="center">
 <img src="https://user-images.githubusercontent.com/92359177/146584423-4c7f1d92-a449-4244-a0e7-958bf54a83ef.png" width="300" />
</p>

For occupations, drivers, sports, and art are more favorable to Trump than politics, law, journalists, and science.  

<p align="center">
 <img src="https://user-images.githubusercontent.com/92359177/146584377-ad5c4003-6f8c-4d24-846d-1ce40b19d336.png" width="300" />
</p>

For the party, there are no differences between Republicans and Democrats. It is interesting to note that both Republican and Democrat are in favour of Trump. However, as they present a similar mean compound, the explanation is probably the same as before: newspapers only quote person talking with respect of the president, leading to a bias selection of the quotes (considering that people against the president are more likely to be aggressive in their words). Moreover, we can note that the numbers of quotations is very well balanced.

<p align="center">
 <img src="https://user-images.githubusercontent.com/92359177/146584296-0a9f9ff8-0630-4306-9a04-bfeb449e35a7.png" width="300" />
</p>

Ethnic group are more complicated to analyze considering the number of quotes available: there are only few Asian and Latino-American people are quoted (respectively 17 and 4). Here it seems that the ethnic group the more in favor of Trump are the African American, ahead Caucasian. This is clearly not what was showed by the polls between 2015 and 2020. This result could be explain by the will of Conservative newspapers to improve the image of Trump by quoting African Americans in favor of Trump. But this is only an hypothesis which is probably not enough to explain this result, and it could also be due to limitations of Vader.

In a more general way, it appears that all the mean value are slightly positive, meaning that, on average, the persons are more quoted when they talk positively about Trump, which is rather the opposite of what one would expect. Of course, this also can be linked with the method used by Vader to determine if a sentence is positive or negative. This can introduce a bias in our study, so let's take that in mind when analyzing the results. But this can also be explained by the a respect for the presidential function, leading newspapers to be kind while quoting people talking about the president.

We can also note that there are no extremes. Two hypotheses can be put forward: either the feelings are extreme in the given category and thus the positive and negative compensate each other to give a more nuanced set, or the feelings are nuanced from the start. We can investigate this thanks to the violinplots: in general, we notice that feelings about Trump are widely dispersed between -1 and 1, showing great diversity.

<p align="center">
   <img src="https://user-images.githubusercontent.com/92359177/146587076-3b484bdf-61ae-44f4-a8cb-efd64dee70f6.png" width="800" />
</p>

So far, the results that show an average positive feeling are quite counter intuitive. For that reason, we will compare Vader result with Flair ones. Flair is another pre-trained sentiment analysis method. Contrary to Vader, it only returns “positive” or “negative” while analysing a sentence instead of a compound.
We represented the percentage of negative sentences return by Flair for the previous categories.

<p align="center">
   <img src="https://user-images.githubusercontent.com/92359177/146587778-6c19fa52-4b37-4876-a4d3-f618c5b1312f.png" width="800" />
</p>

Immediately, it appears that the categories have a more negative opinion to Trump than the Vader ones. This nuances our analysis with Vader where we said that overall the sentiment towards Trump was slightly positive.  
Vader is an algorithm that is rather optimized for social media data, whereas Flair is an algorithm trained on a dataset with larger topics (more specifically on IMDB dataset which is an online database of information related to films, television series, home videos, video games, and streaming content online). Moreover, Vader is a method that only cares about individual words and completely ignores the context in which it is used, while Flair considers the context. One could therefore think that here the results obtained with Flair are more correct, and this is also more in line with what we expect to get about Trump.  
Furthermore, we see that, globally, we find the same difference as before when we compare the labels for a given category. It is rather "reassuring" concerning the results.  
The disadvantage of Flair, however, is the lack of an error bar to better judge the differences.

These results are overall results from 2015 to 2020. But is there a difference in approval rating when we compare before and after Trump election?

<p align="center">
   <img src="https://user-images.githubusercontent.com/92359177/146588657-44bc07a3-8a09-49f4-a4c8-dececdf8cbd8.png" width="800" />
</p>

There is no obvious difference. We can however note maybe a slight decrease for North America, men, politics and Republicans. In conclusion, there is either no change or less positive opinion toward Trump over time.

### Trump's popularity in newspapers

Many newspapers and media have quoted Trump directly or people talking about him since the start of his campaign. Ranking the publishers by the number of quotations in both cases can be informative to assess who is talking about Trump. The following table shows the top 10 publishers along with the number of quotations **about** Trump and the political affiliation.

<p align="center">
   <img src="https://user-images.githubusercontent.com/91223105/146590604-f0fba339-71c2-4a7a-a028-bbd79a747548.png" width="500" />
</p>

Except for the fact that all of these publishers are based in the United States, we cannot extract any trend from that table. It seems that the political affiliation of the publishers is not correlated with the number of quotations. Conservative, liberal and non-affiliated media all report quotations about Trump. Repeating the procedure with the quotations **from** Trump being used by publishers yields different results.

<p align="center">
   <img src="https://user-images.githubusercontent.com/91223105/146590678-64d6838b-002d-44e0-a258-30c5204d0756.png" width="500" />
</p>

The first observation is that the number of quotations is much higher, therefore the results can be slightly more trusted. Additionally, it appears that conservative and non-affiliated newspaper quote Trump the most. However, it is not sufficient to clearly state that either the conservative over-promote Trump or that the Liberals do not quote him on purpose. The missing part of the analysis is the actual content of the quotes.

Intuitively, the idea that all publishers quote content related to Donald Trump is not surprising. After all, he was the president of the United States at the time. However, it may seem plausible that the conservative newspapers would depict him more positively than the liberal ones. Conversely, the opposite has been observed, for instance, when Trump withdrew the accreditation of the journalist Jim Acosta and Fox News, a conservative media commonly known to be highly sympathetic towards him, criticized his decision. The sentiment analysis proposed above can be used to assess this hypothesis.

![image](https://user-images.githubusercontent.com/61464628/146427939-cdb3c37a-05da-48cd-ba37-c4708c557dc1.png)

The figure shown above displays the average Vader compound for the top 10 publishers of quotations **about** Trump. At first glance, it appears that liberal media outlets depict a more positive view of Donald Trump through their quotations. The first conservative publisher only appears in the fourth position. However, the confidence intervals shown in black should be taken into account. Indeed, it can be argued that for a slightly different sampling of the newspaper space, the ranking could have been completely different. Again, the same analysis can be performed for quotations **from** Trump.

![image](https://user-images.githubusercontent.com/61464628/146427978-d1374b67-5ab6-4935-8284-2a60a5f0e009.png)

First, it appears that most publishers have a similar score which is very close to the average score on the entire dataset. Again, the highest ranked newspaper is liberal and the the first conservative one ranks four. However, similarly to the previous paragraph, the confidence intervals, even though they are much more narrow, still indicate that the ranking is quite arbitrary. It seems that the quotations from or about Trump are not well correlated with the political affiliation of the publishers who decides to cite them. To get an idea of the big picture, it can be informative to plot the average Vader compound as a function of the number of quotations for the entire dataset, regardless of the political affiliations.

![image](https://user-images.githubusercontent.com/61464628/146428033-59fc19be-42c8-4f56-9788-688bebf10364.png)
![image](https://user-images.githubusercontent.com/61464628/146428045-710a2df9-735f-4829-8cb4-0e92e5c7196b.png)


These figures speak for themselves. It clearly appears that the sentiment associated to the quotations converges to a slightly positive value in both cases. For sure, a region of extreme opinions can be observed in both plots but they correspond to an interval of small number of quotations which is therefore extremely noisy. 

Finally, it seems reasonable to validate the analysis using an another sentiment analysis tool. A similar procedure can be conducted with Flair's predictions by normalizing the number of positive quotations between -1 and 1 for each publishers. Though comparable, this estimator can not be treated as strictly equivalent to the Vader score.

![image](https://user-images.githubusercontent.com/61464628/146428074-352847e5-89cc-4eab-addb-dc8ec7454c56.png)

Even though the mean value is slightly negative this time, a similar pattern as observed above appears: high variance and extreme values in the low number of quotations regime and convergence towards the mean value when the sample size increases. 

In conclusion, the analysis proposed above seems to indicate that the  quotes about and from Trump published by a media is not representative  of its political affiliation. This could be due to respect towards the president or self censorship. Additionally, the  sentiment analysis is probably not perfect, resulting in noisy labels  for which the uncertainty is difficult to characterize. Moreover, it can be observed that the results of this analysis is coherent with the previous section in which we found that the difference between the sentiment analysis of the quotations about Trump were not significant between democrats and republicans. Finally, one could point out that this conclusion is not really surprising as the  sentiment of the quotations about and from a single man, however famous and power he is, is a weak signal: characterizing the affiliation of a publisher based on this estimator sounds like a shortcut and our analysis shows  that it is indeed one.


# Conclusion

Part 1 ....  
Trump's popularity is better before his campaign and decreases over time. It can be noted that this popularity also depends on the population groups. For example, Asia has worse feelings towards Trump than Europe, Australia and North America, or politicians have worse feelings than sports and movies. Interestingly, the political parties do not have very different opinions. However, it is important to keep in mind that some bias may exist in the choice of quotes in Quotebank from the start.
Part 2....  
Phrase finale
