# stock-analysis
Challenge #2 - Green Stock Analysis

## Purpose:

The purpose of this analysis is to compare the 2017 and 2018 performance of select "green stocks" as requested by Steve to present to his parents.  Steve's parents are interested in investing solely in Daqo and Steve would like to run a performance comparison with other "green stocks" during a two year time period in order to provide his parents investment recommendations.  The original code and refactored code is used to run the analysis with details of performance indicated in the report below.


### Code Refactoring and Analysis

The original code written to perform the analysis required to produce the ticker, volume and performance was written in a way that scanned all cells to produce the required information.  While the code was effective, it was not efficient.  While running the original code did not take a significant amount of time based on the limited analysis required, it would become laggy if the search parameter is expanded to include additional stocks and additional years.  In order to resolve the performance issue, the refactored code is written in a way to only scan and total each individual stock listed in the ticker index.  By limiting the scanning parameters the runtime is significantly reduced and the effectiveness of the script is not hindered.  Screen shots of the run time for 2017 and 2018 as well as results for both unrefactored and factored code have been added to the stock-analysis GitHub repository for reference.

### Advantages and Disadvantages of Refactoring Code

There are both advantages and disadvantages to refactoring code.  The primary advantage is the increased efficiency in executing the code, which is especially useful when dealing with large databases.  There can be several disadvantages to refactoring code.  The first disadvantage is the additional time in takes to rewrite the code in order to increase effiency.  Refactoring code only makes sense if the original code has a long run time, the code was not written in an efficient manner in the first place or if the code and database are long.  In the case of a simple code, refactoring may not make sense based on effort required versus increase in output efficiency.  There is also a potential that refactored code will not look at all required data.  This means that in order for the code to run efficiently the data set would need to be properly sorted prior to running the code.  This was the case for our "green stock" analysis, but often times data is not cleaned and filtered.  This would also have to be taken into consideration when deciding to refactor code as data wrangling and clean up may be a more efficient use of the coder's time if working with a tight deadline.
