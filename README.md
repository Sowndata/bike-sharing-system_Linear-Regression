# bike-sharing-system_Linear-Regression
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider **BoomBikes** has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

- Which variables are significant in predicting the demand for shared bikes.
- How well those variables describe the bike demands

Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

### **Business Goal:**

**To model the demand for shared bikes with the available independent variables.** This will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. **Further, the model will be a good way for management to understand the demand dynamics of a new market.**

### **Highlights**


- There are four categorical variables namely  - season, mnth, weekday, weathersit - which requires mapping and string value assignment

- Created dummy variables for all the categorical variables and have eliminated the redundant first columns as well as dropping few columns such as 'casual','registered'

- Split the data in 80:20 proportions and have done it with appropriate  random sampling.

- Scaled the variables and have selected only the numerical columns to scale and also the scaling is done after the test-train split

- Used RFE and have selected top 15 variables eliminating the rest unwanted variables.

- Checked multicollinearity using VIF and have dropped those features which have a VIF greater than 5

- The two important factors of the final model are complexity and the Adj R-square value. Your model is not simple enough with 10 variables or less.  It has 13 variables but the Adj r- squared value is 0.809 which is very close to the ideal solution.

- Checking the normality of the error terms by plotting a histogram.

- Scaled the test data appropriately using min-max scaler and you have used only transform for this scaling and used this scaled data for predictions and the Adj r-squared value of 0.823 is very close to the solution.

- The Adj r-squared values of 0.809 and 0.823 for the train and test data sets are pretty close to each other and the difference is very low. thus it indicates a good model
