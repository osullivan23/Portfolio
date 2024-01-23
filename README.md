# Charlie O'Sullivan Portfolio
A showcase of personal skills and projects relevant to my career as a Data Analyst 

# About Me
I have a background in science, this is where I first realised the power that lies in drawing valuable insights from the right data. Paramount to the success of my dissertation was taking 1000s of images of galaxies, applying machine learning pipelines to extract parameters, fitting various models to data distributions, and using stats to assess the plots. 

With this amount of data to work with, I realised the importance of selectivity to reveal clear actionable insights. The project helped to confirm that dark matter behaves in a certain way within galaxies, thanks to careful statistical analysis. It was during this project I realised I wanted to pursue a career in data (analysis, modelling, science), and have gained valuable experience in working with big data, Python, and more recently have found the power of BI tools like Tableau and Power BI. 

I live in Sydney and have fallen in love with Australia. I am now looking for the right role to begin a vibrant and rewarding career in data!
# Projects

## Sentiment Analysis of News Channels with YouTube API 
[Source Code](https://github.com/osullivan23/Sentiment-Analysis-News-Channels-YouTube-API-Project/blob/main/yt_api_sentiment.ipynb)
### Overview

This project explores the relationship between sentiment and popularity in the YouTube content of a news channel, utilising the YouTube API. The analysis involves collecting up-to-date data from selected YouTube channels, cleaning the data for sentiment analysis, and utilising the Natural Language Toolkit (nltk) in Python for text processing. The ultimate goal is to understand how the intended sentiment of the content aligns with the audience's reception.

### Project Goals

1. **Data Collection**
   - Create an API client.
   - Develop a framework to extract relevant data from channels of interest using the YouTube API's documentation.
   - Build Pandas DataFrames containing information about videos and comments for each channel.

2. **Data Cleaning**
   - Identify and handle missing data appropriately (remove, interpolate, or extrapolate).
   - Format dates (e.g., convert YYYY-MM-DDTHH:MM:SSZ to the day published).
   - Clean descriptions and comments for sentiment analysis (remove punctuation, emojis, and web addresses).

3. **Distributions of Statistics**
   - Present key statistics about the channels.

4. **Sentiment Analysis**
   - 4.1 **Natural Language Processing (NLP)**
      - Lemmatise text (convert plural forms to singular).
      - Remove stopwords for more meaningful analysis.
      - Part of Speech Tagging (POS) to label each word based on function within text.
      - Named Entity Recognition to identify names, locations, etc.
      - Chunking to group tokens with commonality.
   - 4.2 **VADER Sentimental Analysis**
      - Calculate collective sentiment values.

### Getting Started

### Data Collection - The YouTube API

1. **Register for API Access:**
   - Create a project on the Google Developers Console.
   - Enable the YouTube Data API to obtain API credentials, including an API key.

2. **Understand the API Documentation:**
   - Visit the YouTube Data API documentation for details on endpoints, parameters, response format, and usage guidelines.

3. **Choose the Appropriate Endpoint:**
   - Use the API documentation and a channel's unique ID to locate the data.

4. **Authentication:**
   - Include your API key in API requests for authentication, usually as a parameter in the request URL.

5. **Make HTTP Requests:**
   - Use Python code to make HTTP requests to the API's endpoint. Specify the HTTP method (usually GET) and provide required parameters.

6. **Handle Responses:**
   - Parse JSON responses to extract necessary data. Handle errors and exceptions according to the API documentation.

7. **Rate Limiting:**
   - Stay within YouTube API's rate limits to avoid temporary blocks. Be aware of quotas for different API endpoints and methods.

### Dependencies
- Python
- Natural Language Toolkit (nltk)
- Pandas

### Key Results
- Title, description, and comment sentiment for each news channel. 
- Distribution of views, comments, likes for each video
- Plots showing sentiment vs views. Showing the sentiment which leads to the most views for each channel.
- Word clouds showing the most used title words of each channel. Some use more distressing words than others, e.g. terror, bombing, kidnapping.

### Findings
- The distribution plots revealed that some news channels are successful by stirring up the audience with titles and descriptions geared towards more negative sentiment. Others put out positive content and are successful. But one thing was consistent, more sentimentally positive or negative compared to neutral got a bigger interaction from the viewers (more views, more comments).
- The word clouds revealed the focus of different channels, some would focus on war and distressing topics, and some aim for more positive content. These plots were surprisingly revealing as a first glance.


### Acknowledgements
- Steven Bird, Edward Loper, Ewan Klein for the Natural Language Toolkit (nltk).
- O’Reilly Media Inc. for the book "Natural Language Processing with Python" by Steven Bird, Edward Loper, Ewan Klein.

## Analysing Sydney's AirBnB Market, Visualisation in Tableau
[See dashboard](https://github.com/osullivan23/Portfolio/blob/main/dashboard_AirBnB.png)
I have been exploring new data visualisation tools beyond Python. I love how interactive the dashboards are in Tableau allowing you to constrain data samples and edit outputs in real time. I see the advantages of this in presenting to a client and having the capability to tailor plots to their evolving needs. 

🏠 Intrigued by the Impact of Housing Costs, I Decided to Dive into Sydney's Airbnb Market.

### Insights
   - What did I find? The Airbnb landscape in Sydney's Eastern Suburbs is quite fascinating. The data revealed some intriguing insights.

   - I found that the price per night was most in the north-east of my sample (Vaucluse at the highest latitude is an obvious outlier at over $2000/night average price) as well as the southern shoreline of the harbour. The lowest cost areas are found at lower latitudes with properties averaging close to $200 per night as far south as Maroubra. Being further from the northernmost or easternmost part of the sample reduces the price, due to more considerable distances to the sea.

   - From an investor's point of view, you can see the best returns per bedroom occur for larger properties (4+ bedrooms), or single-room properties at the lower end of the budget. 2 or 3-bedroom properties offer smaller returns per room, 5/6/7 beds offer higher returns per room than entire 2-bed properties, presumably this is skewed as they are likely to be more luxurious properties in this range of bedrooms.

   - We can also see that there is a higher proportion of unoccupied listings in July and August, compared to high occupation in the Australian summer months.

   - This project allowed me to investigate the features offered by Tableau and expand my skill set to include a new approach to visualisations - this is something I will value moving forward due to the quality and variety of displays that can be created in real-time. I can see the power this brings when doing face-to-face consultations with clients, simple commands can be used to edit the data included (suburbs, number of rooms, price range etc.), and create new plots within a matter of seconds.

   - It would be interesting to bring in property purchase prices and long-term rental prices, from another source to complete the picture of the market. For this analysis, I chose Airbnb's API providing up-to-date, and relatively clean data, making the process smoother. I found errors in the datasets and dealt with them appropriately to minimise the effect of biases.

## Comparing the Accuracy of Machine Learning Models
[See Jupyter Notebook](https://github.com/osullivan23/Portfolio/blob/main/heart-attack-knn-dt-lr%20(5).ipynb)
### Overview
I set out to investigate the effectiveness of different types of supervised machine learning models when applied to the task of predicting if, based on a patient's vital signs, they are likely to have a heart attack. I trained a K-nearest-neighbors (K-NN), Decision Tree and Logistic Regression model using the same dataset. These three models use very different approaches 
   - **K-NN** is a machine learning algorithm used for classification and regression tasks, it groups k nearest points by distance.
   - **Decision Tree** is a machine learning algorithm that recursively splits data into subsets based on the most significant feature at each node, forming a tree-like structure for decision-making and predictive modelling.
   - **Logistic Regression** is a machine learning algorithm used for binary classification that models the probability of an instance belonging to a particular class by applying the logistic function to a linear combination of input features.

### Steps

   - Visualise data distribution, head, target variable, feature distributions (continuous, categorical?)

   - Obtained correlation between each feature and the target variable, this was used to identify key features which do need to be included, to avoid overtraining, features with low correlation are excluded from the training features.
   - Scale the parameters so that all values are standardised, to have a mean of 0 and standard deviation of 1. Having the parameters on the same scale allows them to contribute similarly, preventing bias towards certain features as well as increasing performance and improving convergence of the cost function.
   - Split data into training and testing data sets
   - Using scikitlearn’s built in features, I built the models and trained them using the training data (features, x,  and target variable, y)
   - Input the features, x, in the test data set to get the predicted y values (heart attack  predicted or not predicted). 
   - Compare this to the actual y values for the test data to get an accuracy value (percentage)
   - Plotting the Receiver Operating Characteristic (ROC) curve shows us the proportion of true positives vs false negatives. The closer the corner is to the top left of the plot, the greater the accuracy. This works for binary classification models (such as logistic regression and decision tree), but a different method is required for k-NN.
   - To fit the k-NN model best, k is changed and the model retrained and reassessed with each value (3 through to 30), note that even k values lead to issues as the majority of a class may not be obvious e.g. if k=4, having two values of heart attack likely and 2 values of heart attack unlikely means a tie has occurred, it is better to avoid this as it complicates things.
   - Next, the user can input the patient's medical details (age, sex, chest pain, resting blood pressure, cholesterol, fasting blood sugar, resting ecg results, maximum heart rate achieved (thalach), exercise-induced angina, old peak, slp, caa, thall). The models will predict if the person is likely or unlikely to have a heart attack.

## Results
   - Accuracies: Decision Tree 78.6%, Logistic Regression 85.2%, k-NN 93.4%
   - The k-nearest-neighbors model with k=6 produces the highest accuracy (93.4%) and k=5 or k=7 produce accuracy in the region of 92%.
   - The high accuracy achieved makes this a useful tool for medical staff to take someone's vital signs and know whether the patient is in danger of having a heart attack or not. 

# Skills and Achievements
   - Statistics (confidence tests, bayesian stats, fitting models)
   - Numerical skills (integration, differentiation, formulating solutions to complex problems)
   - Computing software competence: (Python, SQL, Tableau, AI).
   - GIS project creating plans for a wind farm in rural NSW ([link](https://github.com/osullivan23/Portfolio/blob/main/Wind_farm_propsal_QGIS.pdf)
   - Python: Pandas, object-oriented coding, matplotlib and seaborn vis, big-data, simulation.
   - Won the Millet award. A £5000 grant was given to three students at the University of Surrey in support of their dissertation project.
   - Lived in three different countries (England, Canada, Australia).
   - Won the local rugby league with my home team before the pandemic.
   - Ran city2surf last year, aiming for the Sydney marathon later this year!

# Certifications
   - [Data Analysis with Python](https://www.freecodecamp.org/Charlie_OSullivan), projects: Arithmetic Formatter, Time Calculator, Budget App, Polygon Area Calculator, Probability Calculator [My code for these projects](https://replit.com/@osullivan23).
   - [Scientific Computing with Python](https://www.freecodecamp.org/Charlie_OSullivan), projects Certifications, Mean-Variance Standard Deviation Calculator, Demographic Data Analyzer, Medical Data Visualizer, Page View Time Series Visualizer, Sea Level Predictor [My code for these projects](https://replit.com/@osullivan23).
   - [Supervised Machine Learning (Regression and Classification)](https://www.coursera.org/account/accomplishments/verify/CLX5PH7HV688)

## License
This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code as needed. Contributions are welcome!
