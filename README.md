Description
This Python script analyzes YouTube comments to derive sentiment insights, potentially applied to Nestlé-related content. It uses the YouTube Data API to extract comments and leverages text analysis libraries to identify sentiment trends and concerns.

Key Functionalities:
Setup and Libraries:

Installs and imports required libraries:
google-api-python-client: For accessing the YouTube Data API.
textblob: For sentiment analysis.
pandas: For data handling and analysis.
nltk: For natural language processing tasks, such as stopword removal.
Downloads NLTK's stopwords for text preprocessing.
YouTube Data API Integration:

Uses an API key and video ID (VIDEO_ID) to fetch comments from a specified YouTube video.
The script interacts with the API through the googleapiclient.discovery library.
Comment Extraction:

Defines a function fetch_comments that retrieves up to 100 comments (modifiable) for a given YouTube video.
Processes the API's response to extract and store comments.
Sentiment Analysis:

Analyzes the sentiment of each comment using TextBlob, categorizing it as positive, neutral, or negative based on polarity.
Insights and Concerns:

Uses NLTK's stopword removal and Counter to analyze recurring words in comments, identifying common concerns or themes.
Potential Applications:
Sentiment Tracking: Understand public sentiment toward a Nestlé product or campaign.
Content Analysis: Identify key themes or concerns in customer feedback.
Marketing Insights: Improve campaigns based on consumer sentiment trends.
Libraries Used:
google-api-python-client: To fetch YouTube comments.
TextBlob: For sentiment analysis.
pandas: To store and manipulate comment data.
nltk: For preprocessing text and identifying common themes.
