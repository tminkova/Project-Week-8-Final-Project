<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100"/>

# Real Estate Market in city of Riga
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
* What would be better: to rent out or to sale, in Riga based on this particular dataset?
* It can help property owners to decide which is better for their investment if they doubt but also to show them some prediction of the prices on the market.
* Splitting the data in training set (80%) to train the model and test its accuracy on unseen data, the testing set (the remain 20%)

## Dataset
* The data is downloaded from Keggle website on my computer, using Pandas to read it in Jupyter Notebook so I can work with it (pd.read_csv('../data/riga_re.csv'))
* The dataset contains 4689 real estate objects in Riga and total 13 columns (data types: float64(6), object(7))
  
  Columns description:
  - op_type (object) - offer type ('For rent', 'For sale', 'Buying', 'Renting', 'Change', 'Other').
  - district (object) - district, where real estate object located.
  - street (object) - address of real estate object.
  - rooms (object) - number of rooms.
  - area (float64) - living area of real estate object.
  - floor (float64) - floor of rel estate object.
  - total_floors (float64) - total amount of floors in building.
  - house_seria (object) - house design ('LT proj.', '602.', 'P. kara', 'Jaun.', 'Specpr.', 'Hrušč.', '119.', 'M. ģim.', 'Renov.', '103.', nan, 'Priv. m.', '467.', 'Staļina',                              '104.', 'Čehu pr.').
  - house_type (object) - type of building ('Brick-Panel', 'Panel', 'Wood', 'Masonry', 'Brick', 'Panel-Brick').
  - condition (object) - stuffing premises ('All amenities', 'Partial amenities', 'Without amenities').
  - price (float64) - price in EUR.
  - lat / lon (float64) - latitude and longitude of real estate object.



## Cleaning
- First, I dropped the 'street' column as it doesn't give me any information for my goals.
- Then, I dropped the rows with missing values as they were less than 10% from the total records because otherwise they could decrease the performance of the model.
- After that, I combined the insignificant values from columns with too many unique values without many records for each of them so it's easier to work with the data.
- Also, I transformed the 'rooms' column from 'object' to numeric so I could see if it's related to the price.
- After checking the correlation of each column to the price, I dropped the unnecessary columns.
- At the end, I split the dataset in 2 different ones - for sale and for rent.

## Analysis
* I used the function 'value_counts' for all of the columns which gave me a good picture what kind of data I'm working with.
* Checked the distribution and took care of the outliers.
* Used Tableau to visualize the GPS coordinates of each listing on the city map.
* Checked the correlation of the numeric values towards the price.
* Which helped me to select the best features for the model.

## Model Training and Evaluation
* First, I split the data in training set 80% to 20% testing set.
* Used features highly correlated to the price.
* Used different models to get the best score possible.
* Used a function for evaluate the results.

## Conclusion
* The best results were shown in the very beginning with the default parameters of Linear Model, yet, I tried to improve them with testing different options (model, parameters, features)
* The question I wanted to answer is way more sophisticated then the results but it's a start in the right direction.
* For the purposes of this project and the time given to implement the new-learn skills my findings are quite satisfying.

## Future Work
It is a great beginning of a bigger project which I would like to work on. It inspired me to collect similar (and even better) data for my region and see how it could be applied in reality.

## Workflow
1. Trello board with the plan
2. Data exploring and cleaning
3. Data preprocessing
4. Splitting and scaling the data
5. Creating and testing different models
6. Changing features and parameters and testing again
7. Creating presentation based on my work

## Organization
I used Trello board to organize the whole process of work.
The repository contains:
- 3 datasets, the initial one and the two I created - one 'for rent' and the other one 'for sale',
- 3 Jupyter Notebooks respectively the datasets,
- a '.gitignore' file
- README file

## Links

[Repository](https://github.com/tminkova/Project-Week-8-Final-Project)  
[Slides](https://www.canva.com/design/DAEe76bdL4k/g6HyPCYmkWpWdCDoOJq-wg/edit?layoutQuery=real+estate+presentation)  
[Trello](https://trello.com/b/WGTw5Rhg/final-project)  
