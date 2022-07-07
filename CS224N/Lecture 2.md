# CS224N NLP with deep learning
## Lecture 2 Word Vectors, Word Senses, and Neural Network Classifiers
### Word2vec parameters
#### A bag of words model
+ The model does not care about word order, but gives the same prediction at each position. 
#### Optimization
For all parameters:
$$
\theta^{new} = \theta^{old} - \alpha\nabla_{\theta}J(\theta)
$$
For one parameter:
$$
\theta_j^{new} = \theta^{old}_j - \alpha\dfrac{\partial}{\partial \theta_j^{old}}J(\theta)
$$
+ Stochastic gradient descent: Use repeated sample windows, (batches) instead of the whole corpus of data
#### Model variants:
+ Skip grams: predict context words given a center word
+ Continuous bag of words: predict center word from a bag of context words. 
+ Negative sampling: train binary logistic regression for the true pair (given center word and context word) and a noise pair. (random sample from vocabulary)
#### SGNS
Overall objective function:
$$
J_{neg}(u_o,v_c,U) = -\log \sigma(u_o^Tv_c) - \sum_{k\in \{K samples\}} \log\sigma(-u_k^Tv_c) \\
\sigma (x) = \dfrac{1}{1+e^{-x}}
$$
Maximize the probability that the real context word appears $\log \sigma(u_o^Tv_c)$ and minimize the probability that the random word appears $\log\sigma(-u_k^Tv_c)$.   
Negative samples are taken with $P(w) = \dfrac{U^{\frac{3}{4}}(w)}{Z}$, the unigram distribution $U(w)$ normalized over the vocabulary, so that less frequent words are sampled more often. 
### Why not build co-occurrence matrix directly?
Word-document co-occurrence matrix will give general topics (latent semantic analysis).  
These high dimensional-vectors are sparse and will make the model less robust. Low and dense dimensional vectors are better.
#### Singular Value Decomoposition 
Take any matrix, and decompose it into three matrices. Then some part of the matrix can be deleted.   
For extremely frequent words, we can log the frequencies/throw away high values/ignore function words
### GloVe moedel
+ Meaning components can be encoded as co-occurrence probability. 
+ log-bilinear model:

$$
w_i\cdot w_j = \log P(i|j) 
$$
so that:
$$
w_x\cdot (w_a-w_b) =\log \dfrac{P(x|a)}{P(x|b)}
$$

Loss function:
$$
J = \sum_{i,j=1}^Vf(X_{ij})(w_i^T\tilde{w}_j + b_i + \tilde{b}_j-\log X_{ij})^2
$$
$X$ is the co-occurrence matrix, $f$ is used to cap the effect of high-frequent words.
### Evaluations of word vectors
#### Intrinsic evaluation
+ Analogy problem
$$
d = \argmax _i \dfrac{(x_b-x_a+x_c)^T x_i}{||(x_b-x_a+x_c)||}
$$
+ Word vector distances and correlation with human judgments
#### Extrinsic evaluations
### Word senses and ambiguity
Idea: clustering word windows around words, retrain word vectors for bank1, bank2, etc.   
Generally, one vector per word type works well. 