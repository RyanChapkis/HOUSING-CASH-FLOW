## PROJECT OVERVIEW:
This model predicts a districts median housing price. It is fed to another Machine Learning system along with other signals in order to determine the cash flow of real estate, and therefore allows for the client to determine whether it is worth investing in real estate in a given area or not. Currently, a districts housing prices are estimated manually by experts, however this process is costly and time consuming, not to mention that their estimates often lack in accuracy (in some cases estimates are off by more than 10%). This model addresses this issue through using census data to train a model to predict a district's median housing price given the other data included with the census. The census data includes the median housing prices of thousands of districts, as well as other data. In this particular example, the California Housing Prices dataset from the StatLib repository was used, which is based on the 1990 California census. Logically, median income was found to be the largest predictor in housing prices. A final RMSE score of 47,766 was obtained which is fine tuned from the original RMSE of 55,564.

### PERFORMANCE MEASURE:
Given that this problem uses regression, Root Mean Square Error (RMSE) gives a good idea of how much error the system makes in its predictions.  

### PIPELINE
Upstream Components -> District Data -> District Pricing (This component) -> District Prices -> Other Signals -> Investment Analysis => Investments 
