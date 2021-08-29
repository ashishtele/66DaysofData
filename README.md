# 66 Days of Data by Dr. Joshua Starmer

> 🌍 The below repository contains the concepts and explanations provided by Dr. Joshua. I tried to collect all the information in one place for quick reference. 🌍

---
# Getting Started
---

[![Challenge Clearly Explained](video_1.PNG)](https://www.youtube.com/watch?v=aOOaGLa8s4c&ab_channel=StatQuestwithJoshStarmer "Explained")

> 🎥 Click the image above for a video!


## [Day1 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6816393714005544960-H2oX)

Diving into CatBoost. CatBoost converts categorical predictors into continuous predictors instead of using one-hot encoding.

<p align="center">
  <img width="650" height="400" src="/images/day1.jpg">
</p>

## [Day2 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-statquest-bam-activity-6816736668716978176-H_TL)

CatBoost has a unique boosting strategy (called Ordered Boosting) that separates the residuals associated with a row of training data from the trees that were built with that row of training data

<p align="center">
  <img width="650" height="400" src="/images/day2.jpg">
</p>

## [Day3 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6817037032859197440-eVeq)

CatBoost does not use normal Decision Trees. Instead it uses Oblivious Decision Trees (ODTs). These are weaker learners (and boosting is all about weak learners) and very fast from a computation side of things.

<p align="center">
  <img width="650" height="400" src="/images/day3.jpg">
</p>

## [Day4 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6817417262551633920-hO5G)

Although normal Decision Trees can handle relationships among features just fine, Oblivious Decision Trees do not. However, CatBoost uses Feature Combinations to try to deal with that.

<p align="center">
  <img width="650" height="400" src="/images/day4.jpg">
</p>


## [Day5 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6817895670515609600-XGOd)

If you have a ton of data, building a tree with it all will take a long time. LightGBM reduces the amount of data used to build each tree using Gradient-based One-Side Sampling (GOSS) to speed things up!

<p align="center">
  <img width="650" height="400" src="/images/day5.jpg">
</p>


## [Day6 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6818221056885624832-r3WK)

Because small residuals are under-reprsented in training datasets, small residuals are amplified by a weight when calculating Gain.

<p align="center">
  <img width="650" height="400" src="/images/day6.jpg">
</p>


## [Day7 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6818608509215670272-vonm)

The more features you have, the longer it takes the train a tree. To reduce the number of features, features not declared as categorical that have relatively little overlap are merged via Exclusive Feature Bundling.

<p align="center">
  <img width="650" height="400" src="/images/day7.jpg">
</p>



## [Day8 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6818894509536030721-6bgB)

LightGBM builds trees "leaf-wise", which, given restrictions on how big the tree can be, generally results in a more accurate tree. This is a big contrast to CatBoost which intentionally builds weaker trees.

<p align="center">
  <img width="650" height="400" src="/images/day8.jpg">
</p>


## [Day9 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6819252799373656064-CYlv)

In contrast to both XGBoost and CatBoost, LightGBM has yet another way to deal with categorical features. I'm looking forward to doing a StatQuest video comparison of these three methods soon!

<p align="center">
  <img width="650" height="400" src="/images/day9.jpg">
</p>


## [Day10 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_right-to-explanation-activity-6819575528434003968-gmIr)

The Right to Explanation - the legal right to be given an explanation for the output of an algorithm. For example, if you are rejected for a loan, you can demand an explanation, and this requires explainable AI.

[Right to explanation](https://en.wikipedia.org/wiki/Right_to_explanation)


## [Day11 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6820023684187648000-sjv6)

One step towards explaining machine learning results is calculating Shapley Values.

<p align="center">
  <img width="650" height="400" src="/images/day11.jpg">
</p>


## [Day12 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6820429161958580225-cl6s)

Joshua naively thought that if he could calculate a Shapley Value for a 1 feature decision tree, he could do it with 2. Nope! However, this motivated creation of SHAP, which are used to explain ML.

<p align="center">
  <img width="650" height="400" src="/images/day12.jpg">
</p>

## [Day13 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6820791056896991232-2GoV)

Joshua figured out how SHAP values are calculated for trees!!!

<p align="center">
  <img width="650" height="400" src="/images/day13.jpg">
</p>


## [Day14-15 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6821540455231094785-QrfV)

A summary of the Main Ideas in SHAP!!!

<p align="center">
  <img width="650" height="400" src="/images/day14_1.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day14_2.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day14_3.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day14_4.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day14_5.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day14_6.jpg">
</p>

## [Day17 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_the-illustrated-word2vec-activity-6822223750692438016-SbL1)

The Illustrated Word2vec [Link](https://jalammar.github.io/illustrated-word2vec/)


## [Day18 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6822631490459889664-EqJL)

A bunch stuff about RNNs, including a chapter from an Neural Networks and Deep Learning by Aurélien Géron. [Link](https://learning.oreilly.com/library/view/neural-networks-and/9781492037354/ch04.html)

## [Day19-20 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6822979701917700097-KQJZ)

Recurrent Neural Networks (RNNs)


<p align="center">
  <img width="650" height="400" src="/images/day20_1.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day20_2.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day20_3.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day20_4.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day20_5.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day20_6.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day20_7.jpg">
</p>

## [Day22 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_understanding-lstm-networks-activity-6824073252973907968-SwGS)

Long Short-Term Memory (LSTM) networks. Chris Olah @ch402 has a great article on the LSTMs.

[Understanding LSTM Networks](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)

## [Day24 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6824781633162403840-JvSG)

A Bidirectional Recurrent Neural Network

<p align="center">
  <img width="650" height="400" src="/images/day24.jpg">
</p>

## [Day25-26 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_dbscan-activity-6825111993897295872-zQ1m)

DBSCAN (a clustering algorithm) [Link](https://en.wikipedia.org/wiki/DBSCAN) [Link2](https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.121.9220)

## [Day27 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6825873560825860096-FRKV)

DBSCAN (a clustering algorithm)

<p align="center">
  <img width="650" height="400" src="/images/day27_1.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day27_2.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day27_3.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day27_4.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day27_5.jpg">
</p>

## [Day28 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_what-is-feature-engineering-activity-6826242423937622016-oXnW)

Feature Engineering [Link](https://www.kaggle.com/ryanholbrook/what-is-feature-engineering)

## [Day33 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_information-theory-mathematics-activity-6828058344503226368-sgAq)

Entropy [Link](https://www.britannica.com/science/information-theory/Discrete-noiseless-communication-and-the-concept-of-entropy)

## [Day34-35 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_shannon1948dvi-activity-6828418600987103232--1tv)

Shannon's original manuscript describing Entropy [Link](http://people.math.harvard.edu/~ctm/home/text/others/shannon/entropy/entropy.pdf) [Link2](https://plus.maths.org/content/information-surprise)

## [Day38 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_66daysofdata-bam-activity-6829821324211339264-5rjy)

Mutual Information

<p align="center">
  <img width="650" height="400" src="/images/day38_1.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day38_2.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day38_3.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day38_4.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day38_5.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day38_6.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day38_7.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day38_8.jpg">
</p>

## [Day42 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_introduction-to-linear-mixed-models-activity-6831313857181495297-I4wo)

Mixed Models [Link](https://ourcodingclub.github.io/tutorials/mixed-models/)

## [Day44 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_a-visual-introduction-to-hierarchical-models-activity-6831998445335707648-LJVw)

Mixed models visualization [Link](http://mfviz.com/hierarchical-models/)

## [Day58 of 66DaysOfData](https://www.linkedin.com/posts/joshua-starmer-phd-95a554130_joshua-starmer-on-twitter-activity-6837115406214324224-8gcD)

A summary of t-SNE, LargeVis and UMAP

<p align="center">
  <img width="650" height="400" src="/images/day58_1.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_2.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_3.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_4.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_5.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_6.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_7.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_8.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_9.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_10.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_11.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_12.jpg">
</p>
<p align="center">
  <img width="650" height="400" src="/images/day58_13.jpg">
</p>
