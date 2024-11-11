Performed Sentiment Analysis of dataset

Steps:

1. Created train and validation datasets
   - flipkart clothes dataset: test dataset
     - Check head
     - Check shape of dataset
     - Check for data type and memory
     - Check for null values
     - Check for duplicates
     - Check for integrity of variable
     - Check for imbalance
  - flipkart clothes dataset: train dataset
     - Check head
     - Check shape of dataset
     - Check for data type and memory
     - Check for null values
     - Check for duplicates
     - Check for integrity of variable
     - Check for imbalance
  - flipkart clothes dataset: validation dataset
     - Check head
     - Check shape of dataset
     - Check for data type and memory
     - Check for null values
     - Check for duplicates
     - Check for integrity of variable
     - Check for imbalance
  - Combine flipkart_electronics and flipkart_mobiles dataset
     - Sample 10,000 data points from flipkart_electronics
     - Add the sampled dataset to flipkart_mobiles dataset
     - Filtering out sampled datapoints from flipkart_electronics dataset
     - Check info of combined dataset

2. Performed EDA before text preprocessing:
   - Train dataset
     - Plot "ratings" variable
     - Plotting "sentiments" variable top 10 counts
     - Plotting "sentiments" variable bottom 10 counts
   - Validation dataset
     - Plot "ratings" variable
     - Plotting "sentiments" variable top 10 counts
     - Plotting "sentiments" variable bottom 10 counts
   - Test dataset
     - Plot "ratings" variable
     - Plotting "sentiments" variable top 10 counts
     - Plotting "sentiments" variable bottom 10 counts
       
3. Train and validation datasets preprocessing:
   - Text pre-processing: Train dataset
     - New Sentiments column
     - Emoji translaton: No
       - Import libraries
       - tokenize_func
       - remove_punctuation
       - postag_func
       - lemmatize_func
       - Create "no_emoji_reviews" column
     - Emoji translaton - Yes
       - Import libraries
       - Open html file
       - Experiment with single datapoint
       - Extract emoticons and emotions
         - Create extract_emotions function
         - Extract_emotion
         - Check length
         - Check first 5 translated emoticons
       - emoticon_replace
       - remove_punctuation
       - Create "yes_emoji_reviews" column
       - Save train data
     - Stopwords removed - Yes
       - stopwords_remove
       - Create "no_stopwords_reviews" column
       - Save train data
  - Text pre-processing: Validation dataset
     - New Sentiments column
     - Emoji translaton: No
       - Import libraries
       - tokenize_func
       - remove_punctuation
       - postag_func
       - lemmatize_func
       - Create "no_emoji_reviews" column
     - Emoji translaton - Yes
       - Import libraries
       - Open html file
       - Experiment with single datapoint
       - Extract emoticons and emotions
         - Create extract_emotions function
         - Extract_emotion
         - Check length
         - Check first 5 translated emoticons
       - emoticon_replace
       - remove_punctuation
       - Create "yes_emoji_reviews" column
       - Save train data
     - Stopwords removed - Yes
       - stopwords_remove
       - Create "no_stopwords_reviews" column
       - Save train data

4. Performed EDA After text preprocessing:
   - Import libraries
   - Import reviews train dataset
   - Import reviews validation dataset
   - EDA: flipkart_train_reviews
     - Null count - Train data
     - Bar-Chart - "ratings"
     - Pie-Chart - "sentiments"
     - histplot - "sentiments"
     - Worldcloud - "text"
       - Import library
       - Convert: "no_stopwords_reviews" - to list
       - Create word cloud and display
       - Top 10 words
   - EDA: flipkart_validation_reviews
     - Null count - Validation data
     - Bar-Chart - "ratings"
     - Pie-Chart - "sentiments"
     - histplot - "sentiments"
     - Worldcloud - "text"
       - Convert - "no_stopwords_reviews" - to list
       - Create word cloud and display
       - Top 10 words

5. Performed additional text preprocessing
  
6. Created word vectors on corpus which did not include emojis
  
7. Created word vectors on corpus which included emojis (emojis were translated into text)
  
8. Created word vectors on corpus which did not include stopwords
  
9. Created classes like cleancorpustransformer and wordvectors
  
10. Performed class profiling and snakeviz visualization on cleancorpustransformer and wordvectors classes
  
11. Built ML models
