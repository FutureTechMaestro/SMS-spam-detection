
SMS Spam Detection using Deep Learning and NLP
This project focuses on building an SMS spam detection system using deep learning techniques and NLP. Three architectures—Dense Network, LSTM, and Bi-LSTM—were implemented and compared to identify the most accurate model for classifying SMS messages as spam or ham.

Dataset:
The SMS Spam Collection dataset from the UCI Machine Learning Repository, containing 5,574 SMS messages (4,827 ham and 747 spam), is used. The data is split into 80% for training (4,000 messages) and 20% for testing (1,574 messages).

Project Workflow
Data Preparation:

Load and explore the dataset to understand spam-to-ham ratios.
Tokenize messages and one-hot encode the labels for processing.
Model Training:

Train Dense Network, LSTM, and Bi-LSTM models using the TensorFlow2 framework.
Evaluate model performance on a validation set.
Model Comparison:

Compare models based on accuracy and select the best-performing one.
Classification of New Messages:

Use the selected model to predict whether new SMS messages are spam or ham.
Results
Dense Network: 98.5% accuracy
LSTM: 98.6% accuracy
Bi-LSTM: 98.8% accuracy (Best Model)
Deployment
A Streamlit app has been developed to showcase the system. Users can input an SMS message, and the app predicts whether it's spam or ham.

How to Use:

Clone the repository:
bash
Copy code
git clone https://github.com/username/sms-spam-detection.git  
Install dependencies:
bash
Copy code
cd sms-spam-detection  
pip install -r requirements.txt  
Download the dataset:
bash
Copy code
mkdir data  
wget https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection -O data/spam.csv  
Train the models using the provided .ipynb script.
Launch the app:
bash
Copy code
streamlit run app.py  


Conclusion
A robust spam detection system was created using NLP and deep learning, achieving a maximum accuracy of 98.8% with the Bi-LSTM model. The model has been deployed through a Streamlit app for practical usage.






