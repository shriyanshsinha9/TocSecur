# TocSecur
TocSecur is an API-based real-time toxic comment detection using Bi-LSTM and dropout layer tuning.
# Problem Statement
To detect different types of toxic comments like threats, obscenity, insults, and identity-based hate. First, we will take the dataset from Kaggle, which consists of Twitter comments, and then we will clear the data of stop words and then train the model to classify the comment in each category.
# Step-wise Algorithm
• Import sequential API - from tensorflow.keras.models import Sequential
• Import all the necessary layers to build the deep neural network - from tensorflow.keras.layers import LSTM, Dropout, Bidirectional, Dense, Embedding
• Instantiate the sequential API - model = sequential()
• Add the Embedding layer using model.add function
• Add the Bi-Directional LSTM layer with an activation function of tanh
• Add the dropout layer with some weight constraint
• Add Feature Extractor fully connected Dense layers using Tanh as their activation functions
• Add the final Dense layer using Sigmoid as the activation function
• Compile the model using Adam as the optimizer
• Train the model using model.fit function for approximately 5 epochs
• Use model.predict to obtain the values for a single input

