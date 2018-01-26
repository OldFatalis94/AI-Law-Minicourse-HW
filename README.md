# AI-Law-Minicourse-HW
##AndreasNotes

###DataCollectionn&PreparationStep1:
+ in 1: code imports packages from Anaconda Distribution, consider HTTP request (user-agent requirement)
+ in 2: code links url of caselaw.findlaw.com, assignment of those cases to variable
+ in 3: code then modifies the variable concerning other factors, like the year of the decision; demands definition of a method in order to execute the url request (grabs requested decisions) and to return the data as an object; optional adding of timeout code; add code for method to grab results within certain range of years in order to receive better results; add code to define method to convert result object into table
+ in(): code results in displaying the corresponding year in the data frame table; by clicking on it, you arrive seeing all decisions of this year (calling function, assigning that to shorthand variable)
+ in(): check table values

###DataCollection&PreparationStep2:
+ in(): code importants packages again
+ in(): code implements output of Step1
+ in(): in order to avoid too many hits, divide data into 3 temporary data frames
+ in(): code implements description of each Supreme Court case, which you can request by clicking on the specific data set
+ in(): code then adds scraped data (case details) to data frame table - do not forget to save!

###DataProcessingStep3:
+ in(): code should now import sklearn stopword list to receive more exact outcome; assign then variables to common words; afterwards, lemmatize all those words; stoplist is applied (text is now cleaned)
