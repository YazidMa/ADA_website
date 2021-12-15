## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/YazidMa/ADA_website/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [Basic writing and formatting syntax](https://docs.github.com/en/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/YazidMa/ADA_website/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.

## What Trump said and what people thought about him from 2015 to 2020

# Abstract

In 2016, the world was completely astonished: Donald Trump was elected president while all the surveys done until this moment estimated Hillary Clinton winner. The four following years were marked by shocking declarations on Twitter, controversies, and withdrawal from previous agreements. But even if this president had been highly criticized by a part of the international community, he was almost ready to run a seond term on 2020. In order to understand better how Donald Trump brought support to his cause, two main parameters must be studied: what was his program before and after his nomination, and how his popularity rating evolved among time.


# Introduction

Three main questions guided this study.
About Trump's program:
-  What were the topics Donald Trump talked about most during the presidential campaign (starting in 2015), and during his time in office (20/01/2017 - 20/01/2021)? Indeed, before looking for Trump's support, we have to understand what he had to offer to his supporters. But studying his official agenda was not as accurate as one could thought, as most of the time, official agendas are "perfect" and should not represent the real thoughts of a candidate. On the contrary, looking for topics that appeared in Trump's quotes over time is much more telling about the goal he pursued. Then, the aim was to look for change over time, for example before and after his election, or because of external events such as the Covid crisis.

About Trump' supporters and opponents:
- Can we quantify Trump's popularity over time? This time, instead of looking for topics in quotes, the idea is to establish whether a quote is in favor or against Trump's policies. Once again, the evolution over time could be linked to external events. Another aspect is the ethnicity of the persons, as Trump's speeches and policies rekindled tensions with minorities.
- In which newspapers are Trump's quotations published? One of the key event of the 2016 campaign was the massive use of both fake news by Russia to discredit Hillary Clinton and tweets to be present on social media. This campaign appears to be a mediatic battle, in which newspapers played a great role. Different information can be provided by this study, as the relation between political affiliation of a newspaper and the positivity of the Trump's quotes it published.

# Method
 
To answer the questions, we needed data. The one we use were extracted by an method described in _Quotebank: A Corpus of Quotations from a Decade of News_ (mettre une référence un peu plus propre ?). Briefly, quotations were extracted from English articles, and their authors were estimated by the program with a confidence value. As the quotation corpus is huge (178 million quotations), the data had to be process smartly to prevent computers from crashing. For that reason, only the data from 2015 to 2020 were selected (one year before Trump's election until the end of his term). Furthermore, only the remaining quotations from Trump or talking about Trump in English were kept. After this preprocessing step, only 1,097,729 quotes remained, which is not negligeable.

# Results

## Trump's main topics over time

More than all other presidents, Trump published many ideas on Twitter, that are then quoted by newspaper. For that reason, most of his ideas are available in our database. To extract them, we just had to consider only the quotations whose author is Trump. At this point, the operation became a bit more complicated: how determine the topics in Trump's quotations? We decided to use [insert the method used], which briefly [insert the mode of action of the methodo used]. The topics were classified into [insert the names of the categories], whose repartition over time is shown below.

[insert the repartition over time of the Trump's topics]

[insert the analysis of the graph above]

## Trump's popularity

### Trump's popularity in the population

During all its political involvement, Trump's was described as a divisive figure. The controversies he created reinforced the adhesion of a part of the population, and reinforced the opposition of the other part. But is this trend visible in quotes from people talking about Trump? The first step was to select only the quotes talking about Trump (means that the quote author is not Trump, but that the word "Trump" appears in the quote). Then, we applied Vader for sentiment analysis. This method allows to determine the degree of posity of a quote, so applying it on the whole dataframe allows to determine the posity of all the quotes. The posity is given by a number between -1 and 1. The closer to 1, the more positive the quotation, the closer to -1, the more negative. 

![image](https://user-images.githubusercontent.com/91223105/146198738-c29b4519-c66f-4a05-b699-6b42755c50d7.png)

One of the first trend we see while looking at this graph is that the peaks are strongly correlated [TODO statistical test?] with small number of quotes for this period of time. To reduce the variance, we decided to group the quotes on a 6 month time window instead of only one month.

![image](https://user-images.githubusercontent.com/91223105/146196478-c876ed0b-a223-492d-97d1-857495fdbf79.png)

This is quite better, the fluctuations are not correlated with the number of quotes anymore! To be sure that our result is in accordance with the reality, we compared our results with a graph of the Trump's popularity rating over time.

[insert, on the same graph, the popularity rating and the previous graph]

[insert comments on the graph above]

Plotting over months can hide general trends over years.

![image](https://user-images.githubusercontent.com/91223105/146194929-20d9242b-d880-4424-b2c6-8dcd83db9dea.png)

It appears that Trump's popularity decreased from 0.22 to 0.15 between 2015 and 2019, meaning a 7% decrease in 4 years. Between 2019 and 2020, his popularity increased to reach 0.19, but this is probably due to the decrease in quotations about Trump, leading to a huge variance in the result (almost 10% against 4% in 2018). As a conclusion, the more time Trump passed in office, the lower its popularity rating.

But is this trend representative of all the American population? Probably not. So to distinguish people that agree or not with Trump policies, we used information provided about the speakers, and especially their ethnicities. Indeed, Trump's term was marked by racial issues like George Floyd death. These problems could have modified the way ethnic groups thought about Trump.


[insert the graph about popularity rate among ethnic groups]

[insert analysis of the graphs above]

### Trump's popularity in newspaper

Many newspapers have quoted personalities talking about Trump since he began the nomination race. The first look inside the data was to assess which newspapers quoted the most people talking about Trump. To compare, we also represented the newspaper quoting the most Trump's word.

[insert table or graph with the main newspapers, and their politial side]

[insert the analysis of the graph above]

However, this analysis is not complete, as a newspaper belonging to the same political side than Trump could report negative words about his policies. That was for example the case when Trump withdrew the accreditation of the journalist Jim Acosta: even Fox News, commonly on his side, criticized his decision. 
As the sentiment analysis was already done for the Trump's popularity over the population, that was not big deal to use it for newspapers. 

![image](https://user-images.githubusercontent.com/91223105/146198115-38d1db66-c1a7-4bd8-a492-2db5c0501d51.png)

There is no general trend, the newspapers seem to quote equaly positive or negative quotes about Trump, whatever their political side. 

We can also analyse the newspapers quoting the most Trump. Here are the newspapers which have the most quoted Trump between 2015 and 2020:

![image](https://user-images.githubusercontent.com/91223105/146193305-b033236b-3b80-4d06-bf59-5057de36a5a2.png)

We notice that these newspapers are quite the same than those who quoted the most people talking about Trump. It seems that these newspapers reported everything related to Trump, meaning both its words than words about him.
However, this means nothing about the support or the opposition of these newspapers to Trump, as they can report positive or negative sentences of Trump. That is why, for each newspaper in the top 10, we represented the average of Trump quote positivity:

![image](https://user-images.githubusercontent.com/91223105/146197657-fa4ddea9-eb36-4f1e-8e0a-8a0eddfe93b6.png)

None of these newspapers reported more positive or negative sentences pronounced by Trump.

# Conclusion
