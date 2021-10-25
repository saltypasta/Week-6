---
tutorial:6
date: 2021-10-19
tags: tag1, tag2, etc
---

# what I was trying to do

_Get familiar with using topic models to shift from Macro and Micro perspectives. Try and find correlations between those two perspectives and tie it all in to the course materials_

+ [Week 6 Repo](https://github.com/saltypasta/Week-6)`

## what I did

+ opened  [topic model](https://programminghistorian.org/en/lessons/topic-modeling-and-mallet#what-is-topic-modeling-and-for-whom-is-this-useful) of 20 000 archaeological articles
	+ Played around a bit with opening the bubbles, looking at the yearly proportion of words in topic and also the overall "Years" heading 
	+ Found this [inflection](obsidian://open?vault=obsidian-digiarch-lab-notebook-main&file=Week%206%2FInflection.JPG) point interesting :
		+ at exactly 1976 there was an sudden increase in publishing of words like: ruler, stela, tikal, date which pushes the other topics to have lower percentages that year
			+ Clicked on this and saw this [graph](obsidian://open?vault=obsidian-digiarch-lab-notebook-main&file=Week%206%2FGraph.JPG)
			+ This correlates with the [inflection point](obsidian://open?vault=obsidian-digiarch-lab-notebook-main&file=Week 6%2FInflection.JPG) mentioned earlier
			+ What was published/happening in 1976 that created this surge?
				+ The [top 4 docs](obsidian://open?vault=obsidian-digiarch-lab-notebook-main&file=Week%206%2FTop%204%20Docs.JPG) of this subject can be found here
				+ The top 2 documents have essentially all of the "tokens" for this subject

+ Switched to [World Archaeology Topic model](http://graeworks.net/digitalarchae/wa/#) to see if any of the words from the previous inflection point correlate
	+ Some of the key words from the previous topic model such as Tikal and Stela had no results in this corpus
	+ Other words like date, temple and Maya had different words associated with them in the world archaeology model than the previous one
		+ ex. Topic Model 1 "Maya": maya classic late american count guatemala ancient period mexico time preclassic postclassic belize antiquity evidence
		+ ex. Topic Model 2 "Maya": ## 3 maya colonial classic spanish belize british indian european san fort indians french race mesoamerican preclassic
+ After using both models, It becomes obvious that the information you include matters in how trends may be represented. A niche subject stood out to me as something that appeared to be very significant, but my best guess was that it was simply the result of one very large document and another fairly large document being published on a niche subject in the same year.  Since several of the subject words such as Tikal did not show up within the World Archaeology journal it appears that it was not significant enough to be mentioned in a "World" scope

```
# example R code
data <- read.csv("data")
```

## challenges 

_I found it hard to read and interpret the graphs since I have little to no experience in statistical analysis. This meant I had to take extra time to stop what I was doing and retrace my thoughts and verify I was interpreting what I was seeing correctly_

## thoughts on where to go next

_Text analysis software may be a useful tool for the graveyard project. I wonder what kind of trends we might find if we were to create a corpus of all of our text data taken from graves. Maybe there would be patterns in the words used by date? or maybe even something more obscure like correlations between different fonts and the gravestone material. That would be fun to play with and see what we could find._


