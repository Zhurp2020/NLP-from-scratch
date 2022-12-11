# CS224N NLP with deep learning
## Lecture 19 Low Resource Machine Translation
### MT in practice
+ Some parallel data are from the origin language, and some in the target
+ Domain of source and target does not match
+ Test/train data are not in the same domain
+ Data collection is very expensive and slow
+ Hard to assess the quality of translation automatically. 
### MT model for English to Napali
+ Add monolingual data in English with noise (swap/drop), and DAE loss
+ Back translation of target side monolingual data
+ Multitask/Multimodality/Multilingual training