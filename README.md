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
• Use model.predict to obtain the values for a single input 
# Flow Chart

![Screenshot 2023-07-30 200846](https://github.com/shriyanshsinha9/TocSecur/assets/126511293/0856c58e-5355-40fc-82da-1b19f0dd8ed0)

# Screenshots


![Screenshot 2023-07-30 201144](https://github.com/shriyanshsinha9/TocSecur/assets/126511293/6bee4241-327f-474f-a284-5ece942f26ee)
<br>

![Screenshot 2023-07-30 201217](https://github.com/shriyanshsinha9/TocSecur/assets/126511293/eeafb06f-142f-4638-a284-85d3bd327683)
<br>

![Screenshot 2023-07-30 201249](https://github.com/shriyanshsinha9/TocSecur/assets/126511293/1ba20caa-24a7-4a33-89ab-dd40814d8014)
