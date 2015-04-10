# Machine Learning 101
@Pycon 2015
Speaker: Kyle Kastner
Fri. 04/10 @ 10:50 AM

Talk materials: https://github.com/kastnerkyle/PyCon2015

## Applications
* Speech Processing
* Image Processing
* NLP
* Advertising
* Recommendations

## Automation Spectrum
### Handcrafted Rules
* if elif elif elif
* DON'T TOUCH code
* Magic constants

### Stats
* linear models
* p values
* Bayesian stats
* MCMC sampling

### Machine Learning
* K-means
* **more**

### Deep Learning
* Neural Networks...
* **more**

## How to organization info

### Manifold Hypothesis
If you think about all the possible images that you could ever see. Most of the informaion that we see is structured and makes sense. Think of specific items like cats and dogs, as opposed to static

### Classification
- This is foo and this is bar.
- Most classification is thought of drawing a boundary in some space.

### Regression
- More

## Learning Functions
This is the core of machine learning. The goal of machine learning is to take some input and get some output. The part in the middle is machine learning.

Example:
- recommend_movies
- french_to_english
- what_is_in_this_image

y = f(x) given theta (Bayes Rules)

## Train/Valid/Test

It is very easy to cheat in ML -- thinking you have done something that someone else hasn't done.

- Split current data
- Evaluate
- Typical Split
 - 80% training
 - 20% validation
- Testing data answers unknown
- Wants systems to work on new data!
- This approach simulated new data

(Think kaggle)

## What should I use?

- [Acanconda](https://store.continuum.io/cshop/anaconda/)
- [Canopy](https://www.enthought.com/products/canopy/)

## Examples

### Recommendations

[ex1_recommendations.ipynb](http://nbviewer.ipython.org/github/kastnerkyle/PyCon2015/blob/master/ex1_recommendations.ipynb)
[ex1_recommendations.py](https://github.com/kastnerkyle/PyCon2015/blob/master/ex1_recommendations.py)

The goal of a recommender system is to recommend something off of the previous thing that was recommended.

Things in this example:
- PMF (Probable Matrix Factorization)
- Users are not unique

![screen shot 2015-04-10 at 11 10 12 am](https://cloud.githubusercontent.com/assets/166734/7090670/a444e3dc-df72-11e4-85aa-ac636bffa42e.png)

### Spam classification

[ex2_spamclassification.ipynb](http://nbviewer.ipython.org/github/kastnerkyle/PyCon2015/blob/master/ex2_spamclassification.ipynb)

[ex2_spamclassification.py](https://github.com/kastnerkyle/PyCon2015/blob/master/ex2_spamclassification.py)

How to train - fit & predict.

### Object detection - Deep neural networks

[ex4_objectdetection.ipynb](http://nbviewer.ipython.org/github/kastnerkyle/PyCon2015/blob/master/ex4_objectdetection.ipynb)

[ex4_objectdetection.py](https://github.com/kastnerkyle/PyCon2015/blob/master/ex4_objectdetection.py)

#### Finding sloths

How do you find sloths in an image?

![screen shot 2015-04-10 at 11 16 29 am](https://cloud.githubusercontent.com/assets/166734/7090747/34b25d78-df73-11e4-82f5-9ecbc5f4138c.png)

#### Sub trees

Is there anything that fits under the subtree?
- Words
- Cats/Dogs

![screen shot 2015-04-10 at 11 16 37 am](https://cloud.githubusercontent.com/assets/166734/7090750/42930758-df73-11e4-8fa5-57ab47215919.png)









