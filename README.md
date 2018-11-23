# ML_theory

In a machine learning problem where the input is denoted by 𝐱 and the output is 𝑦

In order to do machine learning, there should exist a relationship (pattern) between the input and output values. Lets say that this the function
𝑦=𝑓(𝐱), this known as the target function.

However, 𝑓(.) is unknown function to us.  so machine learning algorithms try to guess a **hypothesis** function ℎ(𝐱) that approximates the unknown 𝑓(.), the set of all possible hypotheses is known as the Hypothesis set 𝐻(.), the goal is the learning process is to find the final hypothesis that best approximates the unknown target function.

Different machine learning models have different hypothesis sets, For example the 2d- perceptron has the hypothesis set
𝐻(𝐱)={𝑠𝑖𝑔𝑛(𝑤1∗𝑥1+𝑤2∗𝑥2+𝑤0)∀𝑤0,𝑤1,𝑤2}

The following slide, Courtesy of Prof. Yasser Abu Moustafa Caltech, shows that relationships.
<img src = "https://qph.fs.quoracdn.net/main-qimg-cf260851f899a89ff16a92b38e73729f"/>

