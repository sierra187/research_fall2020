README research_fall2020

Week 1 (09/15 - 09/22):
- Indtroduced to project
- Created database generating function that returns a list of hashed coordinate values


Week 2 (09/22 - 09/29):
- Changed database to be a 2D numpy array that stores a list of hashed coordinate values at each index
- Produced leakage list function, returns a list of queries where each query containts a list of the points with values in the query, some of which are lists of multiple points at the same coordinate.
- Began looking into tensorflow neural net tutorials, looked at classifying MNIST dataset


Week 3 (09/29 - 10/06):
- Wrote function that turns leakage list into 2D numpy array of dimensions (number of queries, length of longest query), this will be what is fed into the neural net
- Looked at another tensorflow neural net tutorial classifying Fashion MNIST dataset, also have been using tensorflow for CNN's in my Deep Learning class


Week 4 (10/06 - 10/13):
- Made function that creates inputs and labels numpy array. Inputs are of shape (number of databases, largest number of queries, length of longest query). Databases are padded so that they are each the same size.
- Started building a neural net using tensorflow and keras. Currently accuracy is very very low.

Week 5 (10/13 - 10/20):
- Added empty queries as row of -1s to leakage, hopefully this will help nn recoginize patterns
- Plotted some of the data to see if any patterns are visually recognizable, there definitely appears to be some patterns between the hashed data points and in the padding and empty queries
- Looked into different types of neural nets
