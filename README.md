## Deploying Flask app into Heroku (Naive Bayes Classification)

This is a demo for a Natural Language Processing Modeling (NLP).

### Dataset
20 newsgroups text dataset that contains roughly 18000 newsgroups posts on 20 topics in which split in two subsets: training and testing.
The split between the train and test set is based upon a messages posted before and after a specific date. (Taken from <a href="https://scikit-learn.org/0.19/datasets/twenty_newsgroups.html">here</a>.)

### Dependencies in deploying Heroku
Some metadata with our application code have to be included, so that Heroku can set up a compatible webserver and install the python packages that our application needs.

#### Installing the gunicorn web server
~~~sh
$ pip install gunicorn
~~~

1. <i>requirements.txt</i> : Specifies the python packages that are required to run our application.
2. <i>Profile</i> : A text file in the root directory of your application that tell Heroku how to start your app.
3. <i>gunicorn.config.py</i> : Optional. Anything specified in this configuration file will override any framework specific settings.

### Demo Instruction:
1. Enter text.
2. Click "Predict" button.

![Demo](/static/img/demo.jpg)
