## Introduction to Deep Learning

### What it is used for?

Everywhere. From things like beating humans in a game, detecting spam in emails, forecasting stock prices, image recognition, diagnosing illnesses - sometimes with more precision that doctors, self-driving cars, etc.

### What is deep learning?

Deep learning is a subfield of machine learning concerned with the algorithms which simulates the function of a brain using artifical neural networks.

### Neural Network

Neural network is the heart of deep learning, it mimicks the process of a brain. A simple neural network is just an object which finds the best line that seperates two data points. Like finding out whether an email is spam or not, here there are only two possiblities, either the email is spam or not. In this case the data-set is simple and simple neural networks may do the job. But in more complex data-sets, we need deep neural networks, i.e combination and layers of simple neural networks.

### Classification Problems

One of the problems we can solve very well with deep learning is classification problems. Like classifying whether an email is spam or not, whether a student is good fit or not, etc.

To do this, we find a line that divides different groups. This line is called a model.
Humans can visually draw a line looking at the graph of data. But to make this happen in computer we make use of different algorithms that finds this line.

Let's say we are classifying students using two parameters, grades and test score, i.e our dataset is in 2-d space and we can easily classify the students using the linear equation, w1X1 + w2X2 + b = 0; If the result of the equation is >= 0 we classify them as accepted, if the result is <0 we classify them as rejected.

Where,
X1,X2 are data points
W1, W2 are weights
b is the bais

Similarly, If we have to judge the students with 3 parameters, i.e our dataset is in 3-d space, we simply extend the linear function to w1X1 + w2X2 + w3X3 + b = 0; now our model is plane, instead of a line.

And, If we have to judge the students with n parameters, we turn the linear function to include all terms upto n.
w1X1 + w2X2 + w3X3 ..... wnXn + b = 0; now our model is a hyper-plane.

### Perceptron

It is the building block of the neural network, it is just a encoding of a linear function. Sometimes the bais is provided as input to the perceptron and sometimes it is within the perceptron.

#### Perceptron Algorithm

The goal of this algorithm is to find the best possible equation that correctly predicts the output (`Y`) for given data points (`X1,..Xn`) by slightly modifying the weights (`W1,..Wn`) and bais `b` with small incremental steps (`learning_rate`).
