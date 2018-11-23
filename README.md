# ML_theory

## INDEX
[Model Representation]()
[What is hypothesis?]()

## Model Representation
First, the goal of most machine learning algorithms is to construct a model: a hypothesis that can be used to estimate Y based on X. The hypothesis, or model, maps inputs to outputs. So, for example, say I train a model based on a bunch of housing data that includes the size of the house and the sale price. By training a model, I can give you an estimate on how much you can sell your house for based on it’s size. This is an example of a regression problem — given some input, we want to predict a continuous output.

The hypothesis is usually presented as
<img src="https://cdn-images-1.medium.com/max/1600/1*XfDb8XhzTy1nVnwSy1mv6g.png"/>

The theta values are the parameters.

Some quick examples of how we visualize the hypothesis:


This yields h(x) = 1.5 + 0x. 0x means no slope, and y will always be the constant 1.5. This looks like:

<img src="https://cdn-images-1.medium.com/max/1600/1*VT2ByIh85TKbdBeZ6uXy8g.png"/>

How about

<img src="https://cdn-images-1.medium.com/max/1600/1*q0zqprvoiRhD4i_51A3JuQ.png"/>

The goal of creating a model is to choose parameters, or theta values, so that h(x) is close to y for the training data, x and y. So for this data

x = [1, 1, 2, 3, 4, 3, 4, 6, 4]
y = [2, 1, 0.5, 1, 3, 3, 2, 5, 4]

<img src="https://cdn-images-1.medium.com/max/1600/1*eHzxmd4mN9YVUts5bXfDFg.png"/>

I will try and find a line of best fit using **linear regression**. Let’s get started.

## Cost Function

We need a function that will minimize the parameters over our dataset. One common function that is often used is mean squared error, which measure the difference between the estimator (the dataset) and the estimated value (the prediction). It looks like this:

<img src="https://cdn-images-1.medium.com/max/1600/1*20m_U-H6EIcxlN2k07Z7oQ.png"/>

It turns out we can adjust the equation a little to make the calculation down the track a little more simple. We end up with:

<img src="https://cdn-images-1.medium.com/max/1600/1*VanG05Ab6yknqJ2bRGFzrQ.png"/>

Let’s apply this const function to the follow data:

<img src="https://cdn-images-1.medium.com/max/1600/1*d0rp7impHwVZn9oJlnEb2w.png"/>




## What is hypothesis?
In a machine learning problem where the input is denoted by 𝐱 and the output is 𝑦

In order to do machine learning, there should exist a relationship (pattern) between the input and output values. Lets say that this the function
𝑦=𝑓(𝐱), this known as the target function.

However, 𝑓(.) is unknown function to us.  so machine learning algorithms try to guess a **hypothesis** function ℎ(𝐱) that approximates the unknown 𝑓(.), the set of all possible hypotheses is known as the Hypothesis set 𝐻(.), the goal is the learning process is to find the final hypothesis that best approximates the unknown target function.

Different machine learning models have different hypothesis sets, For example the 2d- perceptron has the hypothesis set
**𝐻(𝐱)={𝑠𝑖𝑔𝑛(𝑤1∗𝑥1+𝑤2∗𝑥2+𝑤0)∀𝑤0,𝑤1,𝑤2}**

The following slide,shows that relationships.
<img src = "https://qph.fs.quoracdn.net/main-qimg-cf260851f899a89ff16a92b38e73729f"/>

