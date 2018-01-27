# AI-Law-Minicourse-HW
##AndreasNotes

###DataCollectionn&Preparation_Step1:
+ in 1: code imports packages from Anaconda Distribution, considers HTTP request (user-agent requirement)
+ in 2: code links url of caselaw.findlaw.com, assignment of those cases to variable
+ in 3: code then modifies the variable concerning other factors, like the year of the decision; demands definition of a method in order to execute the url request (grabs requested decisions) and to return the data as an object; optional adding of timeout code; add code for method to grab results within certain range of years in order to receive better results; add code to define method to convert result object into table
+ in(): code results in displaying the corresponding year in the data frame table; by clicking on it, you arrive seeing all decisions of this year (calling function, assigning that to shorthand variable)
+ in(): check table values

###DataCollection&Preparation_Step2:
+ in(): code importants packages again
+ in(): code implements output of Step1
+ in(): in order to avoid too many hits, divide data into 3 temporary data frames
+ in(): code implements description of each Supreme Court case, which you can request by clicking on the specific data set
+ in(): code then adds scraped data (case details) to data frame table - do not forget to save!

###DataProcessing_Step3:
+ in(): code should now import sklearn stopword list to receive more exact outcome; assign then variables to common words; afterwards, lemmatize all those words; stoplist is applied (text is now cleaned)

###TopicModelingMethodTesting_Step4:
+ in(): test the current model with LatentDirchletAllocation, Non-negative Matrix Factorization and Latent Semantic Analysis; apply those topic modeling methods and check if all of them reach the right result

###TopicModelingApplicationToData_Step5:
+ 1: running model against the entire dataframe to collect the topics;
* by inserting and executing code, all case descriptions are stacked together to receive one document consisting of all decisions
+ 2: take this model and apply it back to the dataframe to assign most likely topic to each case (we want the topic # and its dot product)
+ 3: make a dictionary of the components that make up each topic from the original model
+ 4: use this dictionary to "look up" the topic components and apply those to the dataframe
+ 5: Getting data together for visualization!
