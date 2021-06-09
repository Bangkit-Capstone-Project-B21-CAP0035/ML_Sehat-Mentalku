# ML_Sehat Mentalku


This program processes users' words through their journals that written in app and Twitter account (if allowed by users).

We use LSTM (Long Short Term Memory) to predict users' conditions based on users' words in the past that we receive. We also use the recurrent neural network (RNN) is a type of artificial neural network commonly used in speech recognition and natural language processing (NLP). RNNs are designed to recognize a data's sequential characteristics and use patterns to predict the next likely scenario.

We need LSTM and RNN so we can use users' past words as input.

Build the LSTM
- To build the LSTM, we need to import a couple of modules from Keras
- Sequential for initializing the neural network
- Dense for adding a densely connected neural network layer
- LSTM for adding the Long Short-Term Memory layer
- Dropout for adding dropout layers that prevent overfitting

As a first step, we need to initiate the Sequential class. This will be our model class and we will add LSTM, Dropout, and Dense layers to this model. The LTSM 64 units which is the dimensionality of the output space. When defining the Dropout layers, we specify 0.1, meaning that 10% of the layers will be dropped. Thereafter, we add the Dense layer that specifies the output of 1 unit. After this, we compile our model using the popular adam optimizer and set the loss as loss. This will compute the binary cross-entropy. Next, we fit the model to run on 20 epochs.

The challenge that we faced is just there was NaN (Not a Number) in the dataset.

We hope this app someday can track users' happiness so we can use it to predict personalized customized users' happiness/trigger lists. Human emotions are fluctuating, so if ML can detect users' extreme mood changes, it will be a great help for therapists giving diagnoses (if any) easier. So in the future, this app can combine CBT therapy and ABCDE therapy so the app can understand and help the users first before any therapist, hopefully.
