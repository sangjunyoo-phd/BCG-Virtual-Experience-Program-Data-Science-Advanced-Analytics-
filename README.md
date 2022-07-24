# BCG-Virtual-Experience-Program-Data-Science-Advanced-Analytics-

# Goal: Build a predict model that gives us insight about who is going to churn the service
sub task: The client also want to know if it is price-sensitive. They are considering a 20% discount that is considered large enough 
to dissuade almost anyone from churning (especially those for whom price is the primary concern).

## 1.	Think about relevant features
* Current Price: Check the Pearson correlation with Churn group to see if churning is a really price sensitive event.
* Contraction types: month-to-month? Year-long contraction? A customer with longer contraction will be less likely to Churn the service.
* Tenure: How long the customer has been contracted with PowerCo? Customers with loyalty to PowerCo will be more likely to be in a longer relationship with PowerCo.
* Country: There could be different regulations/policies in different countries.

## 2.	Exploratory Data Analysis
Categorizing customers looks important task for this topic.
We can start with categorizing customers by current price, such as low, medium, high prices depending on the distribution.
Other categorization criteria should also be considered depending on the features discussed in step 1.
Discount strategy will work better with customers who is already paying high prices for the service and if the churn status is really price sensitive event.

## 3.	Feature Engineering
* Two relational datasets provided. Include price data to client history data.
* Deal with outliers: either by z-score or boxplot
* Some features are highly skewed. Handle them with log(x+1) conversion
* Imbalanced data: use balanced randomforest to categorize Yes Chrun / No Churn customers

## 4. Model Evaluation
* Random Forest: versatile algorithm, no need to worry about overfitting, class-weight included.
* Use Recall (a.k.a. Sensitivity) to evaluate the model. Missing churning clients is going to be critical to the customer.

## 5. Single-slide summary is included.
