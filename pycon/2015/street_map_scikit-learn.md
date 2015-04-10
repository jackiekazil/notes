# Grids, Streets and Pipelines: Building a linguistic street map with scikit-learn

Speaker: Michelle Fullwood
Friday 2:35 p.m.–3:05 p.m.

Talk link: http://us.pycon.org/2015/schedule/presentation/366/

(Missed first 5 minutes)

## Data for classfication

![16478685744_fda20c7043_k](https://cloud.githubusercontent.com/assets/166734/7094787/9f4b8b36-df92-11e4-8c3c-fd833901becc.jpg)

## Ingrediants we need
* Classficiation schema
* Labelled train/test set
* Numberical /Boolean Features
* A classifier
* An evaluation metric

## Classification system
* Malay
* Chinese
* English
* (more)

Labelled train/test set
* Labeled 10% of the data, then used that to classify the next 10%
* Then hand corrected that and used that as the training set
* With this approach, we were able to have less errors as we classified every set of data.

## Choosing features: N-Grams
unigrams
bi-grams
n-grams

![16913350518_45f6173d84_k](https://cloud.githubusercontent.com/assets/166734/7094867/64b9ab82-df93-11e4-9df3-0444b0c031a7.jpg)

## Choosing Features: N-grams
Road names that include bigram 'ck' -- most likely in British.
Different languages have different rates of various n-grams

![16481010593_942b1d0618_k](https://cloud.githubusercontent.com/assets/166734/7094869/680370de-df93-11e4-96eb-323ed5337890.jpg)

Linear support vector classification (SVC)
SVC - we choose the line that has the line that maximizes the space between the two datasets.

![17101167895_497ed59f68_k](https://cloud.githubusercontent.com/assets/166734/7094907/ad448930-df93-11e4-8b8d-7e86d858b619.jpg)

## Adding Features
![17099685622_f0f7cb748c_k](https://cloud.githubusercontent.com/assets/166734/7094906/ad310888-df93-11e4-8b01-1d2591a1e642.jpg)

^^ Has recommended reading.

## Selecting an Evaluation Metric
![16913390058_a06e6941ef_k](https://cloud.githubusercontent.com/assets/166734/7094889/8ea6c0b0-df93-11e4-9d3e-1ffb6dad8190.jpg)

## Add pipelines
![16913681950_d729faf384_k](https://cloud.githubusercontent.com/assets/166734/7095179/292237bc-df96-11e4-9139-e5adbf5b95d9.jpg)

## Adding a new feature to pipeline
![16915050459_1cd7ed46b5_k](https://cloud.githubusercontent.com/assets/166734/7095188/40c7320a-df96-11e4-997f-fd84387b4b72.jpg)

## Adding Feature Union

After adding features...
We got to 65% accuracy

Summary
* Using pipelines and feature unions ...

(Too much info for the time. :-( There is a lot that was missed. This is a very rich talk though and if you are interested, you should go and watch the video.)

** Gridsearchcv **

![16913489068_680424fb29_k](https://cloud.githubusercontent.com/assets/166734/7095200/4abf6692-df96-11e4-9ca0-e4055e4a568e.jpg)

** Making the map **
2 lines of code

![17075310076_1fc0fc358b_k](https://cloud.githubusercontent.com/assets/166734/7095239/9dc2b042-df96-11e4-8aae-df8553919fae.jpg)

![16913494088_4603b4006b_k](https://cloud.githubusercontent.com/assets/166734/7095243/a340f4f2-df96-11e4-9933-94d608ee4f95.jpg)

