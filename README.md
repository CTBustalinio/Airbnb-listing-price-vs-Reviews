# Airbnb-listing-price-vs-Reviews

The objective is to identify reviews and descriptors among expensive, cheap, and neutral AirBnB listings

Data was downloaded from Airbnb, on reviews and listings in San Francisco

An expensive listing is tagged as one if nightly accommodation price >= mean + 0.3 standard deviation of the listings in the neighborhood, per room type. A cheap listing has price >= mean - 0.3 standard deviation

Reviews not in English were excluded in the analysis.

Sentiment Analysis was run on vectorized comments using Multivariate Naive Bayes and Logistic Regression.

Outside the reviews, listing price was predicted using regularized regression and Gradient Boost, but only returned 0.1 R^2.
