<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Title of My Project
*Tsvetelina Minkova*

*Data Analythics, Remote March 2021*

## Content
- [Project Description](#project-description)
- [Hypotheses / Questions](#hypotheses-questions)
- [Dataset](#dataset)
- [Cleaning](#cleaning)
- [Analysis](#analysis)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [Future Work](#future-work)
- [Workflow](#workflow)
- [Organization](#organization)
- [Links](#links)

## Project Description

I used a dataset based on rental properties as well as properties for sale in Riga. 
Real Estate is a big part of my life, not only as a topic of interests but also professionally, I work in property management services for more than 4 years now and I have worked as an independent real estate broker. I embraced the challenge to combine my previous knowledge and experience with the new-learned skills and in this way to enrich my personal passion and enhance my professional capabilities.
My main goal was to create a machine learning model which will predict real estate prices, both for sale and for rent.

## Hypotheses / Questions
* What data/business/research/personal question you would like to answer?
* What would be better: to rent out or to sale, in Riga based on this particular dataset?

* What is the context for the question and the possible scientific or business application?
* It can help property owners to decide which is better for their investment if they doubt but also to show them some prediction of the prices on the market.

* What are the hypotheses you would like to test in order to answer your question?  
* Splitting the data in training set (80%) to train the model and test its aquracy on unseen data, the testing set (the remain 20%)

## Dataset
* Where did you get your data? If you downloaded a dataset (either public or private), describe where you downloaded it and include the command to load the dataset.
* The data is downloaded from Keggle website on my computer, using Pandas to read it in Jupyter Notebook so I can work with it (pd.read_csv('../data/riga_re.csv'))

* For all types of datasets, provide a description of the size, complexity, and data types included in your dataset, as well as a schema of the tables if necessary.
* The dataset contains 4689 real estate objects in Riga.
RangeIndex: 4689 entries, 0 to 4688
Data columns (total 13 columns):
 #   Column        Non-Null Count  Dtype  
---  ------        --------------  -----  
 0   op_type       4689 non-null   object 
 1   district      4674 non-null   object 
 2   street        4237 non-null   object 
 3   rooms         4500 non-null   object 
 4   area          4325 non-null   float64
 5   floor         4356 non-null   float64
 6   total_floors  4345 non-null   float64
 7   house_seria   4247 non-null   object 
 8   house_type    4239 non-null   object 
 9   condition     4283 non-null   object 
 10  price         4219 non-null   float64
 11  lat           4482 non-null   float64
 12  lon           4482 non-null   float64
dtypes: float64(6), object(7)


## Cleaning
Describe your full process of data wrangling and cleaning. Document why you chose to fill missing values, extract outliers, or create the variables you did as well as your reasoning behind the process.

## Analysis
* Overview the general steps you went through to analyze your data in order to test your hypothesis.
* Document each step of your data exploration and analysis.
* Include charts to demonstrate the effect of your work.
* If you used Machine Learning in your final project, describe your feature selection process.

## Model Training and Evaluation
*Include this section only if you chose to include ML in your project.*
* Describe how you trained your model, the results you obtained, and how you evaluated those results.

## Conclusion
* Summarize your results. What do they mean?
* What can you say about your hypotheses?
* Interpret your findings in terms of the questions you try to answer.

## Future Work
Address any questions you were unable to answer, or any next steps or future extensions to your project.

## Workflow
Outline the workflow you used in your project. What were the steps?
How did you test the accuracy of your analysis and/or machine learning algorithm?

## Organization
How did you organize your work? Did you use any tools like a trello or kanban board?

What does your repository look like? Explain your folder and file structure.

## Links
Include links to your repository, slides and trello/kanban board. Feel free to include any other links associated with your project.


[Repository](https://github.com/tminkova/Project-Week-8-Final-Project)  
[Slides](https://www.canva.com/design/DAEe76bdL4k/g6HyPCYmkWpWdCDoOJq-wg/edit?layoutQuery=real+estate+presentation)  
[Trello](https://trello.com/b/WGTw5Rhg/final-project)  
