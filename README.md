# College - CSE4022: Natural Language Processing

### Activity
https://github.com/allenalvin333/College4/blob/master/Project/A1.ipynb

### Project
https://github.com/allenalvin333/College4/blob/master/Project/R3.ipynb

### Labs
- 17th July, 2020 - Frequency and CF distribution<br/>https://github.com/allenalvin333/College4/blob/master/Lab/P1.ipynb
- 24th July, 2020 - Preprocessing: Lexicons and Stemming<br/>https://github.com/allenalvin333/College4/blob/master/Lab/P2.ipynb
- 31st July, 2020 - Text processing pipeline and Web scraping<br/>https://github.com/allenalvin333/College4/blob/master/Lab/P3.ipynb
- 21st August, 2020 - Text classification and Count vectorizer<br/>https://github.com/allenalvin333/College4/blob/master/Lab/P4.ipynb
- 9th October, 2020 - Named Entity Recognition and Domain-specific Jargon<br/>https://github.com/allenalvin333/College4/blob/master/Lab/P5.ipynb
- 16th October, 2020 - Regex parser and Chunking<br/>https://github.com/allenalvin333/College4/blob/master/Lab/P6.ipynb

### File Terminology
- A_: Activity
- DA_: Digital Assignment
- R_: Project
- P_: Lab
  
<br/>
  
# Activity - Comparison of Travel logs using NLTK

### Sources 
-	http://www.natgeotraveller.in/six-years-and-counting/
-	http://www.natgeotraveller.in/train-to-nowhere/
-	http://www.natgeotraveller.in/what-dreams-may-come/
-	http://www.natgeotraveller.in/getting-saucy-about-food/
### Initial framework
-	Converting the text into the digital form: In case the received text is not in a standard digital form. In this case, we scrape data off the internet
-	Tokenization of the text: To segment the given piece of text 
-	Removing Stop words: To remove the non-English set of strings such as the html tags which we get from scraping
-	Taking the word count: To identify the number of words required to convey an idea without reader losing interest
-	Stemming & Lemmatization: To get the root words for better intuition as per what is he/she trying to talk about semantically
-	Vectorization:  we can find out the word similarities/semantics
-	POS Tagging: To differentiate the parts of speech to analyse the advantages and the disadvantages that come along with the excessive use of any POS. 
-	Confidence level > 0.8: Pass: All these parameters contribute to a certain confidence level, and a certain amount of points are required to be qualified
### My contribution
-	Parameter-1: Word count for optimal retention. Here I have considered the limits as 700-750 words for an optimal article and hence the highest confidence score. 
-	Parameter-2: Frequency distribution of words to recognise vocabulary level of the author by seeing the number of repeated words. Under 100 words repeated would give the highest confidence score.
-   Parameter-3: Cosine Similarity. For this, we need to consider multiple documents by the same author. Hence this parameter is not applicable for the confidence scores
-	Parameter-4: Part of Speech tagging for finding an optimal number of adjectives or “beautifying words” to keep the article interesting throughout but still avoid bloating of the real content. The limits are given in terms of the difference between the total number of words versus the number of adjectives, and an optimal number is assumed to be between 600-700
-	Parameter-5: Polysyllabic words do not necessarily increase the complexity of the words, but in a general case, assuming it does, I have given an optimal number to be between 25-35 words with 4 or more syllables
-	Confidence Score: Instead of a regular approach of pass/fail criteria, I’ve embedded score calculation in all the parameters to measure how each article (even if they’re from multiple authors) stand against the requirements/expectations of the employer and the articles qualifying will be mentioned with their scores.
  
<br/>
  
# Project - Racism: Before and After George Floyd

### Scraping
The process of extracting data from a website to retrieve its content. The received input is in HTML format. The tags are cleaned using stopwords and the required segment is saved for further use, usually in a csv format. This is a commonly used technique, the first to do after installing and importing all the necessary packages. I have chosen an article by FSU – Florida State University, to scrape data forgetting the names and coordinates of the capitals of all the states of USA. The scraped data is cleaned, numbers manipulated and allocated into three lists - latitudes, longitudes, and city names
### Sentiment Analysis
The process of interpreting and categorizing the emotion or sentiment conveyed by the speaker in subjective data. Twitter sentiment analysis is for doing the same process, but in a much larger scale with hundreds of thousands of users spread across the country. The centrepiece of this project, the sentiment analysis takes 250 randomly selected tweets per query word given during the call per coordinate points passed and analyses them to give an output whether it is positive, negative, or neutral. All these data are compiled and passed to the next section of the program.
### CSV Write
“Comma separated value” files are commonly used to transfer or exchange data between applications owing to its wide acceptance. It can be viewed in a tabular form and more importantly, it is editable, making the storing of values extremely easy for programs. For my project, the only part to involve this section, is for saving the calculated sentiment values to the corresponding city names and their coordinates. After receiving the calculated value, it will be written into a CSV file and will be called for plotting the chart, later in the program. 
### Display
This segment focuses on showing the calculated values as a visual representation to the viewer. Chart-studio is a great tool in python (and stand-alone) for displaying data in a visual manner using graphs and charts. Here, the saved CSV files contain the name of the city, the location coordinates (rounded off to two decimal places), and the sentiment value (positive and negative in different files) of that query, from that location. From these, the chart-studio tools take the coordinates from all the rows and plot it on the world map (scope = North America). After that, the sentiment values, in terms of percentages, are taken and a circle is plotted on those locations with the radius representing the value 
### Outputs
![Allen1](https://github.com/allenalvin333/College4/blob/master/Images/Project/1.png)
![Allen2](https://github.com/allenalvin333/College4/blob/master/Images/Project/2.png)
![Allen3](https://github.com/allenalvin333/College4/blob/master/Images/Project/3.png)
![Allen4](https://github.com/allenalvin333/College4/blob/master/Images/Project/4.png)
  
<br/>
  
# Author
Allen Ben Philipose
