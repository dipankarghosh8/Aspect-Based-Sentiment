# Aspect-Based-Sentiment
The task is to classify the sentiment of potentially long texts for several aspects. The key idea is to build a modern NLP package which supports explanations of model predictions. The approximated decision explanations help you to infer how reliable predictions are.

## Datasets

The datasets are available at https://drive.google.com/drive/folders/1ZSo7FlaNpEcEyigUX7nmnsYqMsS7FABH?usp=sharing. The downloaded datasets (i.e., the dataset folder) need to be moved into the root path of this project.

Our experimental dataset is `dataset/covid19_tweets.csv`, which is a CSV file contains data about covid19 related tweets. In the CSV file,

- the `user_name` identifies the unique id of the post.
- the `user_location` identifies the veracity of the post, whose value ranges in [ `fake`,  `real`, `unverified`]. 
- the `user_description` is the content of the post.
- 
- the `comments` are the users' comments list towards the post.
- the `content_emotions_labels` and `cotent_emotions_probs` are the *Emotion Category* features of the content. And the `comments100_emotions_labels_mean_pooling`, `comments100_emotions_labels_max_pooling`, `comments100_emotions_probs_mean_pooling`, and `comments100_emotions_probs_max_pooling` are the *Emotion Category* features of the earliest 100 comments. The way how to use these features will be described in [here](https://github.com/RMSnow/WWW2021#step12-get-the-emotion-features).
