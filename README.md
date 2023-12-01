# Brand Sentiment Analysis on Online Cab Services like Ola and Uber using Twitter_Data


![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/0dbff4ad-6354-414b-b99c-5f1722c77dea)


## Table of Contents

- [About](#about)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
- [Data Collection](#data-collection)
- [Data Preprocessing](#data-preprocessing)
- [Model Building](#model-building)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

---

## About

Online Cab Service is a service in which a vehicle is hired with a driver, used by a single passenger or small group of passengers, often for a non-shared ride. This is a service which has been provided by the Companies through Online Application on Android/iOS.
The two cab services whose data we are using for this analysis are Uber and OLA. They have often been found contesting against each other in their claims of owning a majority market share in the country. US-based ride-hailing platform Uber in a recent report claims to have command over 50% of the market share in India. While homegrown ride-hailing player Ola did not share the market share figure it commands in India, the ride-hailing firm recorded 1.5 billion rides on its platform in 2018-19.
A brand sentiment analysis is a process through which you evaluate the audience’s opinion about your brand, services and products. Brands are using Social media for their better customer engagement. Social media sentiment analysis helps to get a grasp of what people think about the campaign.
The rapid growth of online cab services, exemplified by platforms like Ola and Uber, has revolutionized the transportation industry. However, understanding user sentiments towards these services is crucial for service providers to enhance customer satisfaction and make data-driven decisions. Therefore, the problem addressed in this dissertation is the need to conduct sentiment analysis on Twitter data to uncover the positive and negative sentiments expressed by users towards Ola and Uber, identify key pain points, and gain insights into user preferences and concerns. By addressing this problem, service providers can better understand customer sentiments, prioritize improvements, and maintain a competitive edge in the online cab service industry.
- Research Question
  - RQ1. What is the general sentiment of Indian users towards the Online Cab Service (OLA and Uber)? 
  - RQ2. What are the major topics discussed by the Indian users about the Cab-Services ? 
  - RQ3. Identifying the possible reasons of facing issues by the customers through Topic Modelling? 

## Getting Started

### Prerequisites

List the prerequisites that users need to have installed before they can use your project.

- Python 3.x
- Jupyter Notebook (optional for data analysis)/Google colab
- Other dependencies...
## Data Collection

### Data Sources

Twitter's API was utilized to collect a substantial dataset of tweets mentioning Ola and Uber. The collection process involved defining relevant search queries, such as hashtags, keywords, and user mentions, to ensure the retrieval of tweets specifically related to these online cab services. The data collection period and the number of tweets collected were determined to ensure an adequate sample size for analysis.

### Data Preprocessing

Before conducting sentiment analysis, the collected data underwent preprocessing to ensure its quality and consistency. The following preprocessing steps were performed:

- **Text Cleaning**: We removed any special characters, URLs, and unnecessary white spaces from the text data.

- **Tokenization**: The text data was tokenized into individual words or phrases to facilitate further analysis.

- **Stopword Removal**: Common stopwords (e.g., "the," "and," "is") were removed to focus on meaningful words.

- **Lemmatization**: Words were lemmatized to reduce inflected forms to their base or dictionary form, improving the accuracy of sentiment analysis.

## Model Building

In this section, we describe the process of building sentiment analysis models using TextBlob and implementing LDA topic modeling for deeper insights into the textual data.

### Sentiment Analysis with TextBlob

TextBlob, a Python library, was employed for sentiment analysis. TextBlob provides a simple and intuitive interface for sentiment analysis by leveraging the built-in sentiment polarity scoring mechanism. Each tweet in the pre-processed dataset was processed using TextBlob's sentiment analysis functionality, which assigned a sentiment polarity score ranging from -1 (negative sentiment) to 1 (positive sentiment) to each tweet. Sentiment Analyzer, another commonly used sentiment analysis tool, was employed to validate and complement the sentiment analysis results obtained from TextBlob. Sentiment Analyzer is a part of the Natural Language Toolkit (NLTK) library in Python. It utilizes a pre-trained machine learning model to classify text into positive, negative, or neutral sentiment categories. Each tweet in the pre-processed dataset was processed using Sentiment Analyzer, which assigned a sentiment label to each tweet.

1. **TextBlob Installation**:

   To use TextBlob for sentiment analysis, make sure you have TextBlob installed. You can install it using pip:

   ```bash
   pip install textblob
### LDA Topic Modelling
Latent Dirichlet Allocation (LDA), a probabilistic topic modeling technique, was employed to uncover latent topics present in the dataset. The LDA model was applied to the pre-processed tweets, with the number of topics chosen based on prior experimentation and topic coherence measures. The model assigned probabilities to each tweet for belonging to different topics, allowing for the identification of dominant topics within the dataset. The resulting topics were analyzed by examining the keywords associated with each topic cluster. This analysis provided insights into the major themes and discussions surrounding Ola and Uber on Twitter. The identified topics were further validated and interpreted through manual inspection of sample tweets within each topic cluster.

## Results
### Sentiment Analysis on Ola and Uber Tweets:
The sentiment analysis was performed on the collected tweets related to Ola and Uber to gain insights into the overall sentiment expressed by users regarding their experiences with these online cab services. The analysis categorized tweets into positive, negative, or neutral sentiment categories. The following section presents the key results and discusses their implications. 
Below given are the graphs that show our findings on the sentiment analysis on Ola and Uber users:

![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/9ecdb788-b184-4a9e-b540-8c4d7f2f8d54) 
![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/b5d5e05d-52f2-4d13-8d9d-bc0e10a8086a)

### LDA Topic Modelling on Ola and Uber Tweets
The LDA (Latent Dirichlet Allocation) topic modelling technique was applied to the collected tweets related to Ola and Uber to uncover latent topics and gain insights into the key themes and discussions surrounding these online cab services. The analysis resulted in a set of distinct topics, each representing a cluster of related keywords and tweets. The following section presents the main topics identified and discusses their implications.
- Uber

![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/12ec61e5-674f-4861-aa2e-eae44ed3de39)

- Ola

![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/5ae0f3ca-cd62-4e5a-8f8d-ccfc3137f261)

### Topic: Service Quality and Reliability
- Topic Keywords: fail, cancelled, driver, waiting, delay, support

This topic reflects concerns regarding service quality and reliability. Users express frustrations about late arrivals, cancelled rides, waiting times, and delays. This topic highlights the importance of addressing issues related to timeliness and driver availability to enhance customer satisfaction.
 Now, according to our survey, below given is the complete finding of the issue that we are addressing in this topic
![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/e48e563e-4e37-4148-91c1-9dc644c20297)

### Topic: Pricing and Discounts
- Topic Keywords: fare, surge, discount, expensive, return, money

Pricing-related discussions emerge as a prominent topic among users. Keywords such as fare, surge, discount, and expensive suggest conversations about pricing structures and discounts offered by Ola and Uber. This topic indicates the significance of competitive pricing strategies and transparent fare calculations to meet customer expectations.
Now, according to our survey, below given is the complete finding of the issue that we are addressing in this topic-
![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/40ff3902-7b35-4192-be3d-0b62fcbbf32f)

### Topic: App Experience and User Interface
- Topic Keywords: app, interface, user-friendly, navigation, booking

This topic focuses on the user experience of the mobile applications provided by Ola and Uber. Users discuss the app interface, ease of navigation, and overall user-friendliness. Enhancements to the app experience and improvements in features like booking process and real-time tracking can contribute to increased user satisfaction.
Now, according to our survey, below given is the complete finding of the issue that we are addressing in this topic-
![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/195fc380-9fe6-4956-954c-ed0e64661a26)

### Topic: Driver Behaviour and Professionalism
- Topic Keywords: rude, behaviour, professional, driver, customer
Users express concerns about driver behaviour, emphasising the importance of professionalism and courteousness. Keywords such as rude, behaviour, and professional suggest that driver conduct significantly impacts user sentiment. Ensuring driver training programs and maintaining high service standards can address these concerns and foster a positive user experience.
Now, according to our survey, below given is the complete finding of the issue that we are addressing in this topic-
![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/2371f411-c08b-482e-bd89-dfb5f2b37d60)

### Topic: Safety and Security
- Topic Keywords: safety, security, driver, female
Discussions related to safety and security emerges as a key topic, with users mentioning keywords like safety, security, and background checks. This topic underscores the importance of stringent driver screening processes and safety measures to build trust and confidence among users, especially for female passengers. 
Now, according to our survey, below given is the complete finding of the issue that we are addressing in this topic-
![image](https://github.com/roy-rajarshi-27/Brand_Sentiment_Analysis_on_Online_Cab_Services_like_Ola_and_Uber_using_Twitter_Data/assets/126455566/72b48753-a7ed-4f95-822a-9b8736885776)


1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/brand-sentiment-analysis.git
   cd brand-sentiment-analysis
