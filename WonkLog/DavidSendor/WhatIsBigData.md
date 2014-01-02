TheShow

Segment: WonkLog
Scene: What is Big Data?
Talent: David Sendor


---

Hi I'm David Sendor, and I am a Data Scientist. I use data of all types to help people make better decisions. I am especially interested in helping people who do not have tech backgrounds understand the world of data analytics and how to use data to improve their lives.

A term you have probably been hearing a lot these days is big data. 

So What is  Big Data?
 and Why is it so important?

Big Data is a term that describes the combination of a number of different technologies that, WHEN combined, greatly improve our ability to store, process, and analyze huge amounts of data and in doing so learn things that we have never been able to learn before with other techniques.

Because Big Data is so powerful, it is used by many different types of people, who are using it to do many different things, and sometimes talk about it in very different ways. This can get confusing for some people.
For this reason, I believe it is important to understand the concepts behind big data, and to talk about it through an example.

A great example of big data is Google Flu, which is the research Google has done to analyze its users search patterns to predict flu outbreaks.

The US Center for Disease Control, or CDC, tracks the spread of the flu in the US during flu season by location and time and uses its historical data as well as reports from doctors to predict where the flu will spread and when. 

Google took the CDC flu data and compared it to all the searches that its users did on flu symptoms. For example someone might type in “nausea and runny nose”. 

Google found that its search queries can more accurately and quickly predict Flu outbreaks than the CDC data alone. 



This is the promise that Big Data holds. The CDC has brilliant statisticians and doctors who designed an incredibly good sampling and prediction program to track and predict the flu. 

Google though, has more data.



Google Flu is a great example that can show the promises, challenges, and even the dangers posed by big data.

Storing big data
The first technological improvement that has led to Big Data, is our ability to store huge amounts of data very cheaply.

We used to throw out most of our data. Sometimes without even realizing that we were throwing them out.

Think about the hard copy pictures from your childhood and your parents’ childhood.
Some people have them nicely organized and indexed in albums, but most of us have them in shoeboxes. Not easily accessible. 



Then came the digital camera revolution, and we could much more easily store and organize all of our photos.
However, initially the photos that we took were not very good quality.  They were low resolution images. this was partially because the image sensors weren't very good yet, but also because it was expensive to store high resolution photos.  Lower resolution photos throw out a lot of the detail in photos to make them easier to store on a computer and send over the internet.  

These days anyone can store thousands of high resolution photos on their computer or the cloud for very little money.

We are also recording much more information than in the past, due to the ubiquity of cheap sensors such as smartphones and social networks where we store much of our thoughts and experiences in a centralized location.

Think about the number of times that you saw something amazing, for instance your young child says or does something funny, and you wished you had a camera. Now that everyone has a smartphone, those occasions have decreased greatly. But if you think about it, when something amazing happens, and you don't record it, it is stored in your brain, which may be sufficient or even preferable, but in an extreme view of data, you can sort of see not recording this experience as throwing it away.



Google stores a huge percentage of the internet’s data both as indexes to search from and caches or copies of webpages.
According to an estimate by Randall Munroe of xkcd fame, Google has 10 to 15 exabytes of data storage. What does that mean? If you assume that a decently high resolution image is about 1 megabytes, that means google can store more than 2000 pictures for every person on this planet.

Another way of looking at it is that is more than 1 million times the text stored in the books in the Library of Congress. FIX

(assuming the LOC has 10 terabytes of textual data http://en.wikipedia.org/wiki/List_of_unusual_units_of_measurement#Bibles.2C_Encyclopaediae.2C_and_the_Library_of_Congress:_data_volume http://blogs.loc.gov/digitalpreservation/2012/03/how-many-libraries-of-congress-does-it-take/ it is important to note that if one took into account all LOC media, it would be much more than 10 terabytes)

Processing

You cannot just store the data though. You also need to access it and do something with it. 

To handle this much data requires a lot of computing power. 

The biggest advance in this area has been the development of systems that can parrallelize data and processes across multiple computers. 

Let’s say, for example, you are trying to count the number of times Voldemort is mentioned in all 7 Harry Potter books, and you don’t have a computer to count for you.

There are about 1 million words in all 7 books. 
Let’s assume you can scan about 10 words per second, that means it will take you about 28 hours to find all instances of Voldemort. 

Now let’s assume that you have 6 friends who are willing to help you, and you assign one book to each person in your party of 7. Now it will take much less time.  

If each book was the same length, it would take you 4 hours. Since 28 divided by 7 is 4. 

However since some of the books are much longer than others, it will take the person reading the 5th book much longer than the person reading the 1st book, but you will still have a much faster process.

To speed up its search and indexing process, Google created a computer program that very efficiently splits up tasks amongst multiple computers. This program is called MapReduce.

MapReduce and the open source variant of it called Hadoop are one of the biggest factors, if not the biggest factor, that led to the Big Data revolution. 

Think about a Google search for instance. Google farms out its requests to a lot of servers. It is estimated that a single Google search engine query uses 1,000 servers and takes about 0.2 seconds. 
(Quora http://www.quora.com/Google/How-many-processors-does-a-Google-search-query-touch )

This means that if I type in “number of times voldemort mentioned in harry potter” into Google,  I am accessing 1,000 computers at once and getting an answer from Google almost instantly. By the way according to one fan website, Voldemort is mentioned 1,250 times in the books. 
(http://memes.mugglenet.com/Harry+Potter+Funny+Pics/The-Amount-Of-Times-Voldemort-Is-Mention/2401)

Now let’s assume that you are a Google data scientist and are trying to forecast flu outbreaks. The first step would be to look at how common flu related queries in particular area are compared to other non flu related queries in that area.   
(EXPAND?)
This means that you would need to query Google’s database of user searches and find all the times someone searched for a flu related term. 

According to one source that I found (http://www.statisticbrain.com/google-searches/), Google processed almost 2 trillion queries (1,873,910,000,000) in 2012.  That’s 5 billion searches per day and about 60,000 searches per second.  I am not sure if that number is correct, but it is probably around that amount. And that's a lot.

Let’s say that you had a decently fast computer that could search 10 million records per second. At that rate, it would take more than 2 days, just to run your first query of Google searches.

Now Instead, of running the query on one server, Google uses MapReduce to split up the database and has lots of computers do the analysis. It tells the first computer to work on the first 100 million records, the second computer search through the second 100 million records, and so on.  Then, instead of taking 2 days, it takes 20 thousand processors 10 seconds total to finish your query. And frankly, considering Google's computer power and optimizations, it will probably take less than a second for them to do this query.



Finally there is analysis.

The huge amounts of data and the ability to efficiently process that data, has allowed us to perform analyses that were never possible before.

The people doing these analyses are usually called “data scientists”, but that is basically a fancy word for a statistician who uses a lot of computing techniques, or a  computer scientist who uses a lot of statistical techniques.

And frankly, the techniques that are being used are not that new.  While there have been some recent advances in some of the algorithms such as neural networks, which are algorithms designed to mimic the human brain and work particularly well in image recognition, the main technique used by almost every data scientist, least squares regression, was being used in the 1800’s.

The biggest change has been the amount of data that can be applied to these analyses and the speed at which they can be conducted. 
Think about the Google Flu data, we have never before had detailed recorded information that is organized by time and place that shows people's exploratory thoughts on their medical condition without the color and potential biases of a doctor or other expert.

The CDC gets reports from doctors, but not everyone goes to the doctor when they have the flu, they don’t go right away, and the CDC only collects a sample of all doctor visits.

It is much easier to type “do i have the flu” on Google and less than a second later have a search result, than to trudge in to the doctor. Therefore, Google's data contain trends that are likely more comprehensive than the CDC data.


With that said, one still has to be very careful about making predictions from Big Data, because even datasets containing Trillions of records could have biases. For example, Google Flu probably does not do a very good job predicting Flu outbreaks in the Amish community, since they most likely do not use Google. 
I'm sure that if you thought about it, you could also probably come up with some other potential biases in Google Flu.
Even with Big Data,  scientists need to test and validate their predictions and think about the real world implications of the results.




Google Flu also brings up some of the potential privacy issues that Big Data often raises. 

When the AIDS virus first appeared in the 80’s, people did not fully understand how it was transferred, and a lot of AIDS patients were treated very poorly by their friends, family, doctors, and the government. One can easily imagine a dystopian state where you type your symptoms into the search engine and the authorities are banging on your door 15 minutes later. That doesn't mean we should be fearful of Big Data, it just means that we need to design better systems to help protect ourselves from the potentially negative effects of Big Data.


So What is Big Data? 

It is a broad term that discusses the promise from our the ability to track and store more information and to process and analyze it efficiently. 
It is an example of more being better, and the Google Flu example shows how revolutionary its potential is.
but like any amazing new technology, it needs to be applied intelligently, and so I strongly encourage you to learn more about it, about the techniques being used to store, process, and analyze the data, other examples of big data, and the limitations and potential problems with Big Data.


Example Waze
The challenges, promises, and dangers posed by big data can be seen in the rise of the newest mapping  apps most notably Waze.

/*
The velocity of the data, the speed at which it is coming in, has increased significantly. We need faster storage and techniques for handling 

The type of data being stored is also different. Instead of just pictures, or sales data, we have pictures, with comments
Hierarchical systems don’t work as well. 


http://blogs.loc.gov/digitalpreservation/2012/03/how-many-libraries-of-congress-does-it-take/
*/

GPS systems are an amazing tool.
The first generation of GPS systems told you how to get from point A to point B in the fastest time based on the distance and average road speed. In general, this works very well, however it might take you straight into downtown during rush hour
The second generation started to take into account historical traffic and occasionally real time traffic of major routes on an aggregated level. If it is 5 o clock on a weekday, the GPS might know that on average, it takes 30 minutes to drive through downtown, but only 15 minutes to go around downtown.
The third generation adds in the real time speeds of all the cars in the network to get an up to date crowdsourced map of traffic.  
If enough users are using the 3rd generation services, the system will know that there is a car accident well before the news knows it and will be able to start rerouting cars.
The volume and velocity of data required to perform this analysis is incredible.
In generation 1, the system needs to know the map itself, and the road speeds.
In generation 2, the system needs to compute and add the traffic and 
On average, cars traveling through downtown during rush hour take 30 minutes, however a car just took 45 minutes to travel through the downtown area, and the cars in the center of downtown have slowed to a crawl. The system then knows to retoute you.
