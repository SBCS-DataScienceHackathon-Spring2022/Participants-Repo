# SBCS Data Science Hackathon, Competition Two (Simple Classification)

## Table of Contents

1. [Introduction](#introduction)
    - [Schedule](#schedule)
1. [Background](#background)
    - [Programming Languages](#programming-languages)
    - [The Data Set](#the-data-set)
    - [Tasks](#tasks)
1. [Submission](#submission)

## Introduction

For those of you who are returning from competition one, welcome back! We'll be working on scoring all the submissions from last week and releasing the results soon.

For those of you who are just joining now, welcome to SBCS's First Data Science Hackathon! Even though you may have missed the regression competition from last week, you still have the chance to participate in the next three competitions! Before you do, though, please register using [this](https://forms.gle/uMxTnndmVwWWEPZ2A) form. You can also learn more about the hackathon's structure and schedule [here](README-competition-one.md). 

For those of you who participated in competition one but haven't submitted for competition one, don't worry! We've extended the deadline for competition one submissions until 12 PM EDT on April 15th (the same time competition two submissions are due). You can still use the submission links in the [competition one README](README-competition-one.md) to submit your work for the main and side tasks of competition one. **Just make sure you submit your competition two work to the competition two link, not the competition one link in the previous README!!!**

### Schedule

Now that competition one is over, the schedule for the remainder of the hackathon is as follows:
1. Regression (7 days long) : Started at 12 PM EDT on April 1st, now ending at 12 PM EDT on April 15th **(submissions still allowed until then)**.
2. Simple Classification (7 days long) : Starts at approximately 12:05 PM EDT on April 8th and ends at 12 PM EDT on April 15th. 
3. Sentiment Analysis (7 days long) : Starts at approximately 12:05 PM EDT on April 15th and ends at 12 PM EDT on April 22nd.
4. Image Classification (8 days long) : Starts at approximately 12:05 PM EDT and ends at 12 PM EDT on April 30th.

## Background

The second competition focuses on simple classification. Classification is a [supervised learning](https://en.wikipedia.org/wiki/Supervised_learning) practice which invloves using algorithms to classify data into discrete categories based on each data point's observed characteristics (read more [here](https://en.wikipedia.org/wiki/Statistical_classification)). Here, we're focusing on **simple** classification, a term which I am using to mean that the data you'll be using in this competition only contains basic data types, such as integer values, floating point values, characters, strings, Boolean, et cetera. In the next two projects, we'll be using more advanced applications: next week will involve the use of Natural Language Processing (NLP) to some degree, while the final week will involve classifying image data.

### Programming Languages

Just like in the first competition, we expect you to use the Python programming language and the Jupyter Notebook environment because of their extensive popularity and influence in the professional realm of the data science industry.

For those of you who are new to the hackathon, you can use coding environments such as Visual Studio Code and PyCharm Professional **(for which students can obtain a free license, along with licenses to IntelliJ IDEA Professional, CLion, and many more premium JetBrains servoces... more information [here](https://www.jetbrains.com/community/education/#students))** to work with Jupyter Notebook environments. Just make sure to install a recent version of Python on your computer, or the code you write in your Jupyter Notebook (.ipynb file) cannot be processed or executed.

### The Data Set

For this week's competition, you'll be using a Kaggle data set, found [here](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset). It contains medical data for potential stroke patients: age, gender, bmi, et cetera.

### Tasks

Make sure you have Python installed on your computer, as well as an environment that you can use to create and edit Jupyter Notebook (.ipynb) files. Also, make sure you have all the necessary Python data science packages installed on your computer; this can be done using the Python package manager pip, or a third-party service like Anaconda. When you've done this, you can use [this sample](src/task-two-sample.ipynb) to help you get started.

The Main Task once again involves creating a model to beat the baseline model's performance, as defined in the [sample](src/task-two-sample.ipynb). This time, however, the model is a classification model; you'll be using it to try and predict whether or not a given patient suffered a stroke, based on their provided medical data. Because of the purpose that such a model serves, your focus should be on maximizing the number of cases correctly classified as stroke instances, as compared to the total number of actual stroke instances. This means the metric you should be using is recall, which is defined as

<img src="https://render.githubusercontent.com/render/math?math=recall=\frac{TP}{TP - (-FN)}">

where 
  - <img src="https://render.githubusercontent.com/render/math?math=TP"> : the number of true positives (here, the number of patients who did actually suffer from a stroke that were correctly classified as stroke victims by the model).
  - <img src="https://render.githubusercontent.com/render/math?math=FN"> : the number of false negatives (here, the number of patients who did actually suffer from a stroke that were incorrectly classified as not being stroke victims by the model).

**Note: GitHub wasn't processing the standard plus sign in the equation above, so I decided to use a double negative instead. You don't need to calculate it using this formula, Python includes this in the scikit-learn package already.**

The value of recall that you should be trying to beat is in the [sample](src/task-two-sample.ipynb). 

The Side Task is once again focusing on data visualization. You should upload your three best visualization images, just like for last week's competition. 

## Submission 

Please find the submission links for each below:
  - [Main Task: Model Creation](https://forms.gle/WNCz2e3ocKqHttz99)
  - [Side Task: Data Visualization](https://forms.gle/3mCDNHboG7nBt4628)

**Note: the submission links above are for competition two. Please find competition one's submission links [here](README-competition-one.md)!**
