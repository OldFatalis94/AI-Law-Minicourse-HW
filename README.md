# AI-Law-Minicourse-HW
##AndreasNotes

###DataCollectionn&Preparation_Step1:
+ in 1: code imports packages from Anaconda Distribution, considers HTTP request (user-agent requirement)
+ in 2: code links url of caselaw.findlaw.com, assignment of those cases to variable
+ in 3: code then modifies the variable concerning other factors, like the year of the decision; demands definition of a method in order to execute the url request (grabs requested decisions) and to return the data as an object; optional adding of timeout code; add code for method to grab results within certain range of years in order to receive better results; add code to define method to convert result object into table
+ code results in displaying the corresponding year in the data frame table; by clicking on it, you arrive seeing all decisions of this year (calling function, assigning that to shorthand variable)
+ check table values

###DataCollection&Preparation_Step2:
+ code imports packages again
+ code implements output of Step1
+ in order to avoid too many hits, divide data into 3 temporary data frames
+ code implements description of each Supreme Court case, which you can request by clicking on the specific data set
+ code then adds scraped data (case details) to data frame table - do not forget to save!

###DataProcessing_Step3:
+ code should now import sklearn stopword list to receive more exact outcome; assign then variables to common words; afterwards, lemmatize all those words; stoplist is applied (text is now cleaned)

###TopicModelingMethodTesting_Step4:
+ test the current model with LatentDirchletAllocation, Non-negative Matrix Factorization and Latent Semantic Analysis; apply those topic modeling methods and check if all of them reach the right result

###TopicModelingApplicationToData_Step5:
+ 1: running model against the entire dataframe to collect topics
- by inserting and executing code, all case descriptions are stacked together to receive one document consisting of all decisions
+ 2: taking and applying model to the dataframe in order to assign most likely topic to each case
- topic modeling methods then result in specific probability rates, which relate to different topics
+ 3: code creates dictionary for each topic, consisting of 30 words
+ 4: code then uses dictionary to look up topics and applies those to dataframe
+ 5: pivote data in order to visualize it (creating datapoint for every topic for every year)

End of project - fin!
