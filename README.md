<h1>Emotion Detection</h1>
<h2>Overview</h2>
<p>This project focuses on detecting human emotions from textual data using Natural Language Processing (NLP) and Machine Learning techniques.
The goal is to classify text into different emotional categories such as joy, sadness, anger, fear, love, and surprise.</p>
<p>The model analyzes patterns in text and learns distinguishing features that help identify the underlying emotion expressed in the input.</p>

<h2>Objective</h2>
<ul>
  <li>Classify text into multiple emotion categories</li>
  <li>Build a complete NLP pipeline for multi-class classification</li>
  <li>Understand feature extraction using TF-IDF</li>
  <li>Evaluate model performance using standard metrics</li>
</ul>

<h2>Dataset</h2>
<p>The dataset used contains textual data labeled with corresponding emotions.
Each record includes:</p>
<ul>
  <li>Text input</li>
  <li>Emotion label</li>
</ul>
<p>Typical emotion categories include:</p>
<ul>
  <li>sadness</li>
  <li>joy</li>
  <li>love</li>
  <li>anger</li>
  <li>fear</li>
  <li>surprise</li>
</ul>
<p>Dataset Link: <a href="https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp" target="_blank">https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp</a></p>

<h2>Tech Stack</h2>
<ul>
  <li>Python</li>
  <li>Pandas, NumPy</li>
  <li>Matplotlib</li>
  <li>Scikit-learn</li>
  <li>Natural Language Processing (NLP)</li>
</ul>

<h2>Data Preprocessing</h2>
<p>Text data was cleaned and standardized before training the model:</p>
<ul>
  <li>Converted text to lowercase</li>
  <li>Removed URLs</li>
  <li>Removed special characters and punctuation</li>
  <li>Stored cleaned text in a separate column</li>
</ul>
<p>These steps reduce noise and improve model performance.</p>

<h2>Exploratory Data Analysis (EDA)</h2>
<p>Initial analysis and visualizations were performed:</p>
<ul>
  <li>Distribution of emotion labels</li>
  <li>Text length distribution</li>
  <li>Inspection of cleaned versus original text</li>
</ul>
<p>This helped in understanding dataset structure and balance.</p>

<h2>Feature Engineering</h2>
<h3>TF-IDF Vectorization</h3>
<p>Text data was converted into numerical form using TF-IDF:</p>
<ul>
  <li>Transforms text into numerical feature vectors</li>
  <li>Assigns importance to relevant words</li>
  <li>Reduces the impact of commonly occurring words</li>
</ul>
<p>This allows the machine learning model to process textual input effectively.</p>

<h2>Model Building</h2>
<h3>Algorithm Used: Logistic Regression</h3>
<ul>
  <li>Supervised learning algorithm suitable for multi-class classification</li>
  <li>Efficient and scalable for large datasets</li>
  <li>Performs well with high-dimensional sparse data</li>
</ul>
<p>The model was trained on TF-IDF-transformed features to classify emotions.</p>

<h2>Model Evaluation</h2>
<p>The model was evaluated using:</p>
<ul>
  <li><b>Accuracy Score</b> to measure overall performance</li>
  <li><b>Confusion Matrix</b> to analyze predictions</li>
  <li><b>Classification Report</b> including:
    <ul>
      <li>Precision</li>
      <li>Recall</li>
      <li>F1-score</li>
    </ul>
  </li>
</ul>
<p>These metrics provide detailed insights into model performance across all emotion categories.</p>

<h2>Visualizations</h2>
<h3>Emotion Distribution</h3>
<p>Shows the distribution of different emotions in the dataset.</p>
<img src="images/distribution.png" width="600">
<h3>Confusion Matrix</h3>
<p>Displays actual versus predicted classifications.</p>
<img src="images/confusion_matrix.png" width="600">
<h3>Text Length Distribution</h3>
<p>Shows variation in the length of text samples.</p>
<img src="images/text_length.png" width="600">

<h2>Key Insights</h2>
<ul>
  <li>The dataset includes diverse emotional expressions</li>
  <li>TF-IDF effectively captures important textual patterns</li>
  <li>Logistic Regression performs well for multi-class classification</li>
  <li>Specific words strongly influence emotion prediction</li>
</ul>

<h2>Prediction System</h2>
<p>A prediction system was implemented to classify new input text into emotion categories.</p>
<p>The process involves:</p>
<ul>
  <li>Cleaning the input text using preprocessing steps</li>
  <li>Transforming the text using the trained TF-IDF vectorizer</li>
  <li>Passing the transformed data into the trained model</li>
  <li>Mapping predicted labels to corresponding emotion names</li>
</ul>

<h3>Sample Input and Output</h3>


<h2>Conclusion</h2>
<p>This project demonstrates how machine learning and NLP techniques can be used to detect emotions in text.
It showcases a complete workflow from preprocessing and feature extraction to model evaluation and prediction.</p>
