ABSTRACT 

In today’s world, obtaining loans from a financial institution has become a common phenomenon, in this paper we will discuss the profitability of an institution from a business perspective and try to maximize the same, using various machine learning techniques. We will predict loan status based on applications and applicant’s  credit history. Loans taken by a borrower can be fully paid, defaultor charged off depending on a lot of factors out of which some are taken into account.This project will help solve the real world problem by working on the real world data. After this project we will not only have learned about the algorithms needed, but will also understand the importance of data preprocessing and various waysused to do the same. LendingClub is the first peer-to-peer lender to register its offerings as securities with the Securities and ExchangeCommission (SEC), and to offer loan trading on a secondary market.

MOTIVATION

LendingClub is the world’s largest peer-to-peer lending platform.Lending club works as a mediator between investors and borrowers.It works in favour of investors and helps them identify potentialborrowers for lending their money. Potential borrowers are theones who are likely to pay their loans on time. These potential borrowers are identified based on the credit history of the borrower and other application specific factors like interest rates, term ofloan etc. Our project will help solve this issue by using machinelearning techniques.

PERFORMANCE MATRIX

To maximize the profitability of the organization, the best matrix for evaluation was precision of the model. Inside the precision weare more concerned about reducing the number of false positive results.
<ul>
<li>True Positive(TP): These are the candidates which are pre-dicted as potential borrowers by our model and are actually potential borrowers.</li>
<li>False Positive(FP): These are the candidates which are pre-dicted as potential borrowers by our model and have actually defaulted their loans.</li>
<li>True Negative(TN): These are the candidates which are pre-dicted as defaulters by our model and are actually potential borrowers.</li>
<li>False Negative(TN): These are the candidates which arepredicted as defaulters by our model and are actually default-ers.Our main aim while training this model is to minimize the numberof false positive(FP) results, since these are the customers whichcause heavy losses to lending club.</li>
</ul>

CLASSIFICATION

Our classification goal is to predict which class the loan belongsto: either Default or Fully Paid. 
In the following sections, we will share and discuss our experiments using Neutral Networks and Random Forest for classification problem. For metrics to evaluate classification performance, we use confusion matrix whose columns represent predicted values and rows represent true values. We also measure precision, recall, f1-score (the harmonic mean of precisionand recall) and weighted average as defined below:

𝑃𝑟𝑒𝑐𝑖𝑠𝑖𝑜𝑛=𝑇𝑃 / (𝑇𝑃+𝐹𝑃)

𝑅𝑒𝑐𝑎𝑙𝑙= 𝑇𝑃 / (𝑇𝑃+𝐹𝑁)

𝐹1−𝑠𝑐𝑜𝑟𝑒=2 * 𝑇𝑃 / (2 𝑇𝑃 + 𝐹𝑃 + 𝐹𝑁)

𝑆𝑢𝑝𝑝𝑜𝑟𝑡=𝑡ℎ𝑒 𝑛𝑢𝑚𝑏𝑒𝑟 𝑜𝑓 𝑡𝑟𝑢𝑒 𝑖𝑛𝑠𝑡𝑎𝑛𝑐𝑒𝑠𝑓𝑜𝑟 𝑒𝑎𝑐ℎ 𝑙𝑎𝑏𝑒𝑙

𝑊𝑒𝑖𝑔ℎ𝑡𝑒𝑑−𝑎𝑣𝑔𝑚𝑒𝑡𝑟𝑖𝑐 = 𝑚𝑒𝑡𝑟𝑖𝑐 𝑤𝑒𝑖𝑔ℎ𝑡𝑒𝑑 𝑏𝑦 𝑠𝑢𝑝𝑝𝑜𝑟𝑡

CONCLUSION:

We have successfully built a machine learning algorithm to predict the people who might default on their loans. We opted against using Principal Component Analysis for dimensionality reduction since we had a lot of categorical data. This can be further used by LendingClub for their analysis. For our purpose we used Artificial Neural Network, XGBoost and Random forest for our Modelling purpose. Upon doing our exploratory data analysis and using the linear measures of correlation between the predictors and the response, the most important variables for predicting loan defaulters are total mortgage accounts, annual income, installments and loan amount. During the course of our project, we realized some keypoints. Collection of more data points for loan defaulter (false pos-itives) will help us classify them better. Also, we can use otherpre-processing techniques or variables to improve the prediction power of the algorithm. We can also categories the loan defaulters based on how many times they have defaulted. This will help us minimize the false negative which in turn will help us maximize profit.The biggest challenge in the prediction of loan defaulters was the data surrounding the limited number of people who defaulted on their loan. We can use recent data compare the number of current loans that were paid off or defaulted. We should also note the loans that were charged off. Then these new data points can be used for predicting them or even used to train the model again to improve its accuracy. As mentioned earlier, instead of PCA we can use different variable selection techniques like Multiple correspondence
Analysis to further reduce the dimension. This will help us select the most important features. This will enhance the model fit since attributes which are not contributing much to our model will be removed. In the end, our model was able to predict the lending club default rate at a good accuracy and making few changes in pre-processing and reduction in dimensionality we can further improve the performance of our model.


