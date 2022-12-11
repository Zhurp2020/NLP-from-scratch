# CS224N NLP with deep learning
## Lecture 17 Model Analysis and Explanation
### Model analysis at varying levels of abstraction
1. As a probability distribution and a decision function
2. As a sequence of vector representations
3. Parameter weights, mechanism, attention
### Model evaluation as analysis
1. In domain/same distribution test set
2. Diagnostic test set for a specific capacity of the model
3. Test for language properties in language models
4. Evaluate knowledge in models by using prompts
### Saliency map
A score for each word indicating its importance to the model's prediction
### Explanation by input reduction
What is the simplest input to get the same prediction?
### Analyze models by breaking them 
Break models by making seemingly innocuous change to the input  
Test if the model is robust to noise in the input. 
### Analyze components of the model
Train a probe for a specific layer of the model. 