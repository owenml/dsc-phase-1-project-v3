# Phase 1 Project Description - Qi, Olu and Scotty

You've made it all the way through the first phase of this course - take a minute to celebrate your awesomeness!

Now you will put your new skills to use with a large end-of-Phase project!

In this project description, we will cover:

* [***Project Overview:***](#project-overview) the project goal, audience, and dataset
* [***Deliverables:***](#deliverables) the specific items you are required to produce for this project
* [***Grading:***](#grading) how your project will be scored
* [***Getting Started:***](#getting-started) guidance for how to begin your first project

## Project Overview

For this project, we utilized data cleaning, imputation, analysis, and visualization to generate insights for a business stakeholder.

### Business Problem

This company is expanding into new industries to diversify its portfolio. Specifically, they are interested in purchasing and operating airplanes for private enterprises. but do not know anything about the potential risks of aircraft. The company will cater to individual clients, corporations, or groups who require exclusive and personalized air transportation, for business, convenience, luxury, or efficiency reasons.

### The Data

In the `data` folder is a [dataset](https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses) from the National Transportation Safety Board that includes aviation accident data from 1962 to 2023 about civil aviation accidents and selected incidents in the United States and international waters.



## Business Understanding

The company is interested in purchasing and operating jets for business, executive, corporate and private clients.

Our company had several key questions regarding their new business endeavor:

* What are the most reliable types of engines that we can purchase for our aircraft?
* Which aircraft would have the most optimal cost of maintenance and operation?
* Which aircraft have the best outcomes in case of accidents in terms of injuries and aircraft damage?
* What is the financially optimal number of engines per aircraft?
* Which aircraft has features that would best help us serve our clients?



## Data Understanding and Analysis

The interactive dashboard is a collection of views that allows the viewer to change the views to understand different features in the data. This dashboard will be linked within your GitHub repository README.md file so that users can explore your analysis. Make sure you follow visual best practices that you have learned in this course. Below is an example of what you could produce for this assignment.
![tableau dashboard for aviation accidents](https://i.imgur.com/ZjFRMiT.png)

![tableau dashboard for aviation accidents](https://i.imgur.com/n9K3Kwa.png)

![tableau dashboard for aviation accidents](https://i.imgur.com/gzvfViq.png)



***To pass this project, you must pass each project rubric objective.*** The project rubric objectives for Phase 1 are:

1. Data Communication
2. Authoring Jupyter Notebooks
3. Data Manipulation and Analysis with `pandas`
4. Interactive Data Visualization

### Data Communication

Communication is a key "soft skill". In [this survey](https://www.payscale.com/data-packages/job-skills), 46% of hiring managers said that recent college grads were missing this skill.

Because "communication" can encompass such a wide range of contexts and skills, we will specifically focus our Phase 1 objective on Data Communication. We define Data Communication as:

> Communicating basic data analysis results to diverse audiences via writing and live presentation

To further define some of these terms:

* By "basic data analysis" we mean that you are filtering, sorting, grouping, and/or aggregating the data in order to answer business questions. This project does not involve inferential statistics or machine learning, although descriptive statistics such as measures of central tendency are encouraged.
* By "results" we mean your ***three visualizations and recommendations***.
* By "diverse audiences" we mean that your presentation and notebook are appropriately addressing a business and data science audience, respectively.

Below are the definitions of each rubric level for this objective. This information is also summarized in the rubric, which is attached to the project submission assignment.

#### Exceeds Objective
Creates and describes appropriate visualizations for given business questions, where each visualization fulfills all elements of the checklist

> This "checklist" refers to the Data Visualization checklist within the larger Phase 1 Project Checklist

#### Meets Objective (Passing Bar)
Creates and describes appropriate visualizations for given business questions

> This objective can be met even if all checklist elements are not fulfilled. For example, if there is some illegible text in one of your visualizations, you can still meet this objective

#### Approaching Objective
Creates visualizations that are not related to the business questions, or uses an inappropriate type of visualization

> Even if you create very compelling visualizations, you cannot pass this objective if the visualizations are not related to the business questions

> An example of an inappropriate type of visualization would be using a line graph to show the correlation between two independent variables, when a scatter plot would be more appropriate

#### Does Not Meet Objective
Does not submit the required number of visualizations

### Authoring Jupyter Notebooks

According to [Kaggle's 2020 State of Data Science and Machine Learning Survey](https://www.kaggle.com/kaggle-survey-2020), 74.1% of data scientists use a Jupyter development environment, which is more than twice the percentage of the next-most-popular IDE, Visual Studio Code. Jupyter Notebooks allow for reproducible, skim-able code documents for a data science audience. Comfort and skill with authoring Jupyter Notebooks will prepare you for job interviews, take-home challenges, and on-the-job tasks as a data scientist.

The key feature that distinguishes *authoring Jupyter Notebooks* from simply *writing Python code* is the fact that Markdown cells are integrated into the notebook along with the Python cells in a notebook. You have seen examples of this throughout the curriculum, but now it's time for you to practice this yourself!

Below are the definitions of each rubric level for this objective. This information is also summarized in the rubric, which is attached to the project submission assignment.

#### Exceeds Objective
Uses Markdown and code comments to create a well-organized, skim-able document that follows all best practices

> Refer to the [repository readability reading](https://github.com/learn-co-curriculum/dsc-repo-readability-v2-2) for more tips on best practices

#### Meets Objective (Passing Bar)
Uses some Markdown to create an organized notebook, with an introduction at the top and a conclusion at the bottom

#### Approaching Objective
Uses Markdown cells to organize, but either uses only headers and does not provide any explanations or justifications, or uses only plaintext without any headers to segment out sections of the notebook

> Headers in Markdown are delineated with one or more `#`s at the start of the line. You should have a mixture of headers and plaintext (text where the line does not start with `#`)

#### Does Not Meet Objective
Does not submit a notebook, or does not use Markdown cells at all to organize the notebook

### Data Manipulation and Analysis with `pandas`

`pandas` is a very popular data manipulation library, with over 2 million downloads on Anaconda (`conda install pandas`) and over 19 million downloads on PyPI (`pip install pandas`) at the time of this writing. In our own internal data, we see that the overwhelming majority of Flatiron School DS grads use `pandas` on the job in some capacity.

Unlike in base Python, where the Zen of Python says "There should be one-- and preferably only one --obvious way to do it", there is often more than one valid way to do something in `pandas`. However there are still more efficient and less efficient ways to use it. Specifically, the best `pandas` code is *performant* and *idiomatic*.

Performant `pandas` code utilizes methods and broadcasting rather than user-defined functions or `for` loops. For example, if you need to strip whitespace from a column containing string data, the best approach would be to use the [`pandas.Series.str.strip` method](https://pandas.pydata.org/docs/reference/api/pandas.Series.str.strip.html) rather than writing your own function or writing a loop. Or if you want to multiply everything in a column by 100, the best approach would be to use broadcasting (e.g. `df["column_name"] * 100`) instead of a function or loop. You can still write your own functions if needed, but only after checking that there isn't a built-in way to do it.

Idiomatic `pandas` code has variable names that are meaningful words or abbreviations in English, that are related to the purpose of the variables. You can still use `df` as the name of your DataFrame if there is only one main DataFrame you are working with, but as soon as you are merging multiple DataFrames or taking a subset of a DataFrame, you should use meaningful names. For example, `df2` would not be an idiomatic name, but `movies_and_reviews` could be.

We also recommend that you rename all DataFrame columns so that their meanings are more understandable, although it is fine to have acronyms. For example, `"col1"` would not be an idiomatic name, but `"USD"` could be.

Below are the definitions of each rubric level for this objective. This information is also summarized in the rubric, which is attached to the project submission assignment.

#### Exceeds Objective
Uses `pandas` to prepare data and answer business questions in an idiomatic, performant way

#### Meets Objective (Passing Bar)
Successfully uses `pandas` to prepare data in order to answer business questions

> This includes projects that _occasionally_ use base Python when `pandas` methods would be more appropriate (such as using `enumerate()` on a DataFrame), or occasionally performs operations that do not appear to have any relevance to the business questions

#### Approaching Objective
Uses `pandas` to prepare data, but makes significant errors

> Examples of significant errors include: the result presented does not actually answer the stated question, the code produces errors, the code _consistently_ uses base Python when `pandas` methods would be more appropriate, or the submitted notebook contains significant quantities of code that is unrelated to the presented analysis (such as copy/pasted code from the curriculum or StackOverflow)

#### Does Not Meet Objective
Unable to prepare data using `pandas`

> This includes projects that successfully answer the business questions, but do not use `pandas` (e.g. use only base Python, or use some other tool like R, Tableau, or Excel)

### Interactive Data Visualization

Tableau is a powerful data analysis tool that allows data to be presented in a manner that allows it to be easily digestible with visualizations and charts to aid in the simplification of the data and its analysis. Tableau contains many customizable features and makes it easy to share in many ways. We recommend you use Tableau for your interactive data visualization now that you have experience with it.

Here are the definitions of each rubric level for this objective.

#### Exceeds Objective
Creates an easy to use dashboard to answer business questions

#### Meets Objective
Successfully creates a dashboard to answer business questions

#### Approaching Objective
Creates a dashboard, but it is difficult to use

#### Does Not Meet Objective
Unable to create a dashboard 

## Getting Started

Please start by reviewing the contents of this project description. If you have any questions, please ask your instructor ASAP.

Next, you will need to complete the [***Project Proposal***](#project_proposal) which must be reviewed by your instructor before you can continue with the project.

Then, you will need to create a GitHub repository. There are three options:
Interactive Data Visualization
1. Look at the [Phase 1 Project Templates and Examples repo](https://github.com/learn-co-curriculum/dsc-project-template) and follow the directions in the MVP branch.
2. Fork the [Phase 1 Project Repository](https://github.com/learn-co-curriculum/dsc-phase-1-project-v3), clone it locally, and work in the `student.ipynb` file. Make sure to also add and commit a PDF of your presentation to your repository with a file name of `presentation.pdf`.
3. Create a new repository from scratch by going to [github.com/new](https://github.com/new) and copying the data files from one of the above resources into your new repository. This approach will result in the most professional-looking portfolio repository, but can be more complicated to use. So if you are getting stuck with this option, try one of the above options instead.

## Conclusion
This project will give you a valuable opportunity to develop your data science skills using real-world data. The end-of-phase projects are a critical part of the program because they give you a chance to bring together all the skills you've learned, apply them to realistic projects for a business stakeholder, practice communication skills, and get feedback to help you improve. You've got this!

