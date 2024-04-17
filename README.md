# PracticalApplication2-CarDealership
Capstone project 2

Project summary: 

Although my ultimate findings were inconclusive at the time of submission, I found this project to be one of the most fascinating and illuminating of the course so far. 

After extensive data cleaning and preparation, and after using multiple methods to predict both important features, as well as my own intuition, I was able to find one model which produced a significantly lower mean squared error result than the others. 

Sequential Feature Selection repeatedly produced some features which I had suspected would be important drivers in determining price, however, it omitted others which I knew would be important. 

It was my own selection of features which yielded the best results. This was an inflection moment for me. This validated something I have been saying since before enrolling in this class.  "As 'smart' as a machine can be, its intelligence means nothing without a human being to operate, oversee, or to be the most intelligent source of input to a machine learning algorithm." 

I spent a great deal of time on data cleaning and prep. Probably too much considering the 15 hour estimate. (I probably spent 15 hours just cleaning and prepping) 

Again, the biggest difficulty I had on this project was working in isolation. 

I had a tough time determining the 'meaning' of my mean squared error results. Initial models came back with astonishingly high numbers again and again - until finally my own hand-picked set of features came back with a significantly lower number (although it still seemed quite high to me). What does that number mean? How is it calculated considering what is in the data and how I filtered it? 

In conclusion, my thoughts about the best determiners of the price of a used vehicle are the following: 

The year the vehicle was made, the mileage on the odometer, and any data related to the condition of the vehicle. The model I used for prediction which yielded the best results as well as best cross-validation results was a 3rd degree PolynomialFeatures using LASSO. The features I selected (manually) were: 

selected_features = ['year', 'odometer', 'condition_excellent', 'condition_good','condition_fair', 'condition_poor']


My assignment leaves off at deployment. It was my intent to build a function which took a number (a top threshold of vehicle prices), allow the end user to have minimal interaction with the model, and return ballpark estimates of price based on the available data for vehicles on their lot. 

I ran out of time, not so much for personal time constraints, but because there was (is) still so much I wanted to look into with this data. For example, I isolated the data on manufacturer, model, and states. I believe there is a whole secondary study that can be done on regionality and what influence manufacturers (and vehicle models?) have on predicting price. I would love to have worked on this as part of a team! 