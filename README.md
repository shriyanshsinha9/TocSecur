# TocSecur
TocSecur is an API-based real-time toxic comment detection using Bi-LSTM and dropout layer tuning.
# Problem Statement
To detect different types of toxic comments like threats, obscenity, insults, and identity-based hate. First, we will take the dataset from Kaggle, which consists of Twitter comments, and then we will clear the data of stop words and then train the model to classify the comment in each category.
# Step-wise Algorithm
• Import sequential API - from tensorflow.keras.models import Sequential <br>
• Import all the necessary layers to build the deep neural network - from tensorflow.keras.layers import LSTM, Dropout, Bidirectional, Dense, Embedding <br>
• Instantiate the sequential API - model = sequential() <br>
• Add the Embedding layer using model.add function <br>
• Add the Bi-Directional LSTM layer with an activation function of tanh <br>
• Add the dropout layer with some weight constraint <br>
• Add Feature Extractor fully connected Dense layers using Tanh as their activation functions <br>
• Add the final Dense layer using Sigmoid as the activation function <br>
• Compile the model using Adam as the optimizer <br>
• Train the model using model.fit function for approximately 5 epochs <br>
• Use model.predict to obtain the values for a single input <br>

