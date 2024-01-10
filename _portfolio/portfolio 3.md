---
title: "Neural Network Classification Scheme"
excerpt: "Implementing neural network from scratch to predict Hawks bird species based on wing size and weight for a wildlife rehabilitation centre, based at historic Spier Wine Farm <br/><img src='/images/eagle.jpeg'>"
collection: portfolio
---
This project centers around the development of a neural network for species classification based on bird biometric features—specifically, weight and wing size. The neural network architecture includes two input nodes, one hidden layer with eight nodes, and three output nodes representing one-hot encoded species. The primary goal is to predict species based on the given features.
![EDA](/images/finalEDA.png) 

### Key Contributions 
- The softmax function in the output layer is utilized for multi-class classification, providing a probability distribution for species prediction. This function assigns probabilities to each class, allowing for a more nuanced understanding of prediction outcomes.
- In the validation analysis, tanh and RELU activation functions are compared using their respective validation error trajectories. Tanh activation is favored over ReLU, with a validation error generally lower, emphasizing the importance of activation function choice.
- The impact of regularisation on reducing complexity and fitting the model to the data is visually represented.
- Response curve analysis is conducted for tanh and ReLU specifications, showcasing the prediction areas for each species.The ReLU activation function demonstrates a more linear prediction boundary, particularly in classifying species B.

![Both Responses](/images/Bothresponse.png)

In conclusion, the project emphasizes the importance of thoughtful activation function selection and regularization for neural network performance. Insights gained from response curve analysis can guide further model refinement and exploration.

Find the code [here](Wildlife Rehab Centre Project.Rmd)

This project was done in collaboration. 

