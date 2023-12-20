<h1>Breaking BERT: Gradient Attack on Twitter Sentiment Analysis for Targeted Misclassification</h1>
<h2>Overview</h2>
<p>
This project focuses on exposing the vulnerabilities of BERT in the context of sentiment analysis on Twitter. The primary objective is to create a framework for generating targeted adversarial texts that can mislead sentiment analysis models without detection. The framework relies on a white-box approach, utilizing gradients to prioritize the importance of individual words within the text. This fine-grained sensitivity helps pinpoint words with maximal influence on the classification outcome.
</p>
<h2>To run the project</h2>

<ol>
<li> Clone the repository. </li>
<li> Upload all of the notebooks to google colab and upload the data folder to your google drive's root directory.</li>
<li> Preprocess the data by running <b>PreProces.ipynb</b>. (Note that this step is necessary only if you want to re-preprocess the tweets as it has already been done in advance and the file <b>tweets_preprocessed.ipynb</b> is present in the data folder.) </li>
<li> Fine Tune the pretrained bert model on the processed dataset by running <b>Fine Tune.ipynb</b>. It would create a model called <b> tweet_classification</b> which would be uploaded to your drive.</li>
<li> Generate Adversarial Texts for the negative tweets by running <b>Generate Adversarial Text.ipynb</b>. This would create a <b>dumps</b> folder in your drive which would be useful for the following step.</li>
<li> Calculate Post-Attack accuracy by running <b>Post-Attack Accuracy.ipynb</b><li>
</ol>
<br>
<b>Dataset link: </b> https://www.kaggle.com/datasets/yasserh/twitter-tweets-sentiment-dataset
<br>
<b>Pre-trained model: </b> https://huggingface.co/MarieAngeA13/Sentiment-Analysis-BERT 
<br>
<b>Sentence Encoder: </b> https://tfhub.dev/google/universal-sentence-encoder/4
<br>
