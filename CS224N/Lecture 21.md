# CS224N NLP with deep learning
## Lecture 21 Socially intelligent NLP systems
### Toxicity of LMS
+ learning stereotypes and social biases from training data
+ at risk for generating toxicity in <100 generations
### Hate speech detection
+ Dataset are ignoring underlying social dynamics of speech (identity, dialect...), Overt toxicity detection backfires against minorities
+ Detecting identity based on dialect lexical indicators, datasets are biased against AAE
+ Highlighting dialect influences labels of offensiveness. 
#### Annotations
Who, why, what behind toxicity annotations.
+ Racist speech is less offensive to people who hold racist beliefs and anti-censorship ideas. 
+ Swear words are more offensive to conservatives and traditionalists.
#### Social bias frames
+ overt and subtle biases
+ more explainable, trustworthy and holistic than hate speech detection
+ lewdness/offensive/intention/group/in group ...
+ Train a transformer to predict the tags. 
### Power Transformer
Rewrite language to debias it. 
### Avoiding and mitigating language bias with human centric models