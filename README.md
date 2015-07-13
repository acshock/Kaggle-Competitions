# Kaggle-Competitions
I've worked on some kaggle competitions. If you look at the scripts themselves, they're all ipython notebooks. I've
added some annotation so you can see my thought process as I'm working through the competitions. A lot of the 
things I'm trying don't work. I'm hoping that means I haven't been motivated enough to find the right answer. But 
everyone who's wrong hope that.

The forest cover script: 

The problem: given a collection of information about various different types of environments for trees, can you predict the type of tree?

The best solution: I used some basic stats to make a guess about the most important features and how to seperate it into tree type. This allowed me to beat the basic benchmark but wasn't as good as using more advanced techniques.

I stopped working on that one because the deadline for the contest was almost open. I 
wasn't using any publicly available scripts because I didn't have internet access where I was working on it. So 
if it looks extra messy, that's why. I did beat the benchmark using only my reasoning skills and no computer 
modelling.

The eeg model: 

The problem: given a set of data on how the brain responds to someone using their hands to do a specific task, can you predict when someone will do that specific task? Used for making better prosthetics for amputees.

The best solution: someone in that competition had gotten a score of 92% on the first day. I didn't think that there 
was much I could add to that so I stopped working on it. She had prior subject specific knowledge for this type of data.

The Liberty Mutual data: 

The problem: given a set of anonymized data about houses, can you predict how risky it would be to insure the house? If a house is rated as more risky, the company can do further investigations of the home.

The best solution: To be honest, I would be surprised if any of the current solutions accomplish the ultimate goal. Because a large majority of houses don't appear to be incredibly high risks (~75%), it's very hard to predict the houses which do have higher risks and need further scrutiny. If you're going for accuracy (how the competition is scoring), you can get a model that predicts 39% of the results. But my guess is that all the high scorers (aka the items of most interest) will be false negatives...which makes those solutions relatively useless.

Working solution right now: If you can break up all of the data into binary functions (it either is a value or it isn't), is there some way to average over the different data to get a better prediction? For instance, low scorers tend to have more 1s in column 4 than high scorers; high scorers tend to have more 1s in column 8 than low scorers. If I wasn't working in the restraint of the competition, I would break up the risk/hazard scores for the houses into low/mid/high scorers (no/maybe/definitely further investigation, respectively). The models would most likely find the commonalities easier with fewer groups to split the data into which would add more value for the company. My two cents.
