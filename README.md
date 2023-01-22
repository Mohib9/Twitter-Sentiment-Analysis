# Twitter-Sentiment-Analysis

The objective was to understand the politcal sentiment of the pakistani poublic on the political point of view with the data limited to last 6 months of the year 2022.

The data was scrapped from twitter with the search items set to 'Pakistan Politics' and time set to between 1st june,2022 to 31st Dec,2022. The attributes that were extracted included udernames, date & time, likes, source(android, apple, desktop etc), retweets and the content. The data was then converted to .json and .csv to save into the respective folders to access for later use.

The data consisted of 76952 data points with a few NA values as well. The rows that contained such missing values were limited to less than 50 and were hence removed since they would not have made a lot of difference. The tweets also contained other languages such as urdu, punjabi etc. which were identified and translated to english using GoogleTrans library. After the translation, the tweets were cleaned which included tokenization, lemmatization, hashtags, @ and website links.

After the tweets were cleaned, they were identified as positive or negative using the Sentiment Intensity Analyzer in the NLTK library with the consideration of the compound scores as metrics for accessing the polarity. 

Upon closer look, it was found that of the total tweets, the postive tweets were 44%, Negative tweets 39% and tweets which did not pose any sentiment were 16%. 

The sentiment expressed over time was quite stable with a mix of both positive and negative tweets with the exception of extremely negative tweets in the later half of the August. The day to week wise analysis indicated a variation in the overall tweet sentiment with Mondays being more negative as compared to other days of the week. Futhermore, the general overview of the words used throughout the public view remained largely centered on Imran Khan.


