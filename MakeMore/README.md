# MakeMore
A language model which simply generates more of what it has been trained on. In this case, the input provided is a set of names and the task is to create a model and train it such that it would generate names similar to the input.

## What is a bi-gram?
Bi-gram model is a variation of the n-gram model, consider the vocabulary of the input to be the first five alphabets of the english language. All possible pairs formed out of those can be termed as bi-grams. The frequency of occurance of all of these pairs across the provided input is measured and respective probability is calculated. This probability is presented in a then used to predict the next most probable character in the sequence and hence achieving a new generation. 

![image](https://github.com/user-attachments/assets/063eb69f-9022-497b-ba92-90de5a3837cd)

The above image presents the table containing the frequency of bigram appearing in the input. ***'.'*** represents a special characters which marks the beginning and end of a word. This table is used to calculate the probabilty which is used in finding the next most probable character.

## Is the model effective?
This model is initially being trained only on the probabilites (unweighted), the output is consistent in this case but the quality of the output can be understood by calculating the likelihood. 

## Introducing a Single Layer of neurons
To enhance the output efficiency of the model, a single layer containing 27 neurons is created. This portion presents the introdcution of tensors and weights and discusses the intricate details of role of dimensions in Machine Learning applications.

Futhermore, processing of the input using one hot encoding to match the appropriate input as required by the neural network is discussed. Finally, back propagation is used to optimize the weights to emphasize on more relevant bigrams as compared to others. This stage completes one complete forward, backward and parameter updation for the model.

