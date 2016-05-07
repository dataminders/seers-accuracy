###Background Prior to attending this competition
Thakur Raj Anand (DataGeek) : I am a data science analyst with Masters in Quantitative Finance based out of Hyderabad. I mostly use R and Python for data science competitions.

Oleksii Renov (orenov) : I am a data scientist based out of Dnipro, Ukraine. I love to do programming in Python, R and Scala.


####Data Exploration
We spent 40% of the time exploring data and converted the problem into a Supervised problem. We generated negative sample by assigning 0 to those IDs which had no transaction in the year 2006 but had a history before 2006. We constructed 4 different representation of data to make models with the idea of capturing different signals from different representations

####Modeling 
We mainly used XGBOOST but we did try Random Forest and ExtraTrees but they didn't help to improve the final predictions. We made 4 tree models and 1 linear model using XGBOOST. We only made a linear model on the final representation of data on which XGBOOST was giving best CV. 


####Black Magic - Was there any trick to get a significant lift?
Oleksii found that predictions from tree model and linear model were very different and averaging them was giving a significant boost in CV as well as on LB.


####What did you learn from the competition?
We learned a lot about sparse matrices. We decided to learn simple things like aggregating, transformation etc. on sparse matrices which is very helpful in exploring large data sets in  an efficient way.


####Words of Wisdom
Never give up. Try to make a different representation of data and try different models on them.
