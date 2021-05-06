# Identification Of Toxicity Within Text With Hybrid Convolution Plus Gated Recurrent Unit System
<img src="https://www.e-medine.org/wp-content/uploads/2019/12/e-Medine-Europe-Hate-Speech_sito-1400x760px.jpg" width="950" height="520">
<p>With the rise of the internet, social media has now become the central place for spreading hate and toxicity especially in the form of text. This not only leads to the spread of negative and toxic atmosphere but it also highly affect the individuals in form of depression or loss of confidence. To tackle this problem I have created an NLP integrated deep learning system that helps to determine automatically whether a text contains toxicity or not without any human help.</p>
<h2>Libraries Used</h2>
<ul>
  <li>Tensorflow</li>
  <li>Keras</li>
  <li>Numpy</li>
  <li>Pandas </li>
  <li>Matplotlib</li>
  <li>Seaborn</li>
  <li>Numpy</li>
  <li>Sklearn</li>
  <li>Spacy</li>
  <li>BeautifulSoup</li>
  <li>Wordcloud</li>
</ul>
<h2>Word Cloud Representation</h2>
<p align="center">
<img src="https://github.com/NavinBondade/Identification-Of-Toxicity-Within-Text/blob/main/Graphs%20&%20Pictures/Word%20Cloud%20Representation%20Combine.png?raw=true" alt="wordcloud_representation" >
<h2>Target Class Distribution</h2>
<img src="https://github.com/NavinBondade/Identification-Of-Toxicity-Within-Text/blob/main/Graphs%20&%20Pictures/Distribution%20Of%20Dependent%20Variable.png?raw=true" >
<h2>Model Details</h2>
<p>For identification of toxicity, I have created a hybrid model convolution plus gated recurrent unit model. The specialty of this model is that it leverages the benefit of a convolution neural network for feature extraction and learning long-term dependencies of the gated recurrent unit. The model uses one single-dimension convolution layer followed by two gated recurrent unit layers followed by two fully connected neural network layers for decision making. All the layers use RELU as an activation function except the last dense layer that uses the sigmoid activation function to map predicted values to probabilities between 0 and 1.</p>
<h2>Model Traning</h2>
<img src="https://github.com/NavinBondade/Identification-Of-Toxicity-Within-Text/blob/main/Graphs%20%26%20Pictures/Loss%20and%20Accuracy%20Combine.png" alt="loss_accuracy">
<p>The model was trained for 18 epochs. During training, the model uses Adam as an optimizer for performing backpropagation and uses binary crossentropy as the loss function to penalize model more when it makes false predection.</p>
<h2>Model Analysis</h2>
<p>After model training for 18 epochs, the model has achieved an accuracy of 85 % and a loss of 0.2519. (The conclusion here is that if the model trained for more epochs it will achieve more accuracy but due to limited resources I wasn't able to do that.)</p>
<h2>Model Evaluation</h2>
On test data, the model has achieved a loss of 0.97 and an accuracy of 70%.

To tackle the spread of toxicity on the internet that many times leads to depression in many people I have built a deep learning system that determines whether a text contains toxicity or not.
