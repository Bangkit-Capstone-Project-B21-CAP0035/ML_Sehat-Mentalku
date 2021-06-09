# ML_Sehat-Mentalku

This program processes users' journals.

We use LSTM (Long Short Term Memory) to predict users' conditions based on users' words in the past that we receive. We also use the recurrent neural network (RNN) is a type of artificial neural network commonly used in speech recognition and natural language processing (NLP). RNNs are designed to recognize a data's sequential characteristics and use patterns to predict the next likely scenario.

We need LSTM and RNN so we can use users' past words as input.

Build the LSTM
- To build the LSTM, we need to import a couple of modules from Keras
- Sequential for initializing the neural network
- Dense for adding a densely connected neural network layer
- LSTM for adding the Long Short-Term Memory layer
- Dropout for adding dropout layers that prevent overfitting

As a first step, we need to initiate the Sequential class. This will be our model class and we will add LSTM, Dropout, and Dense layers to this model.

The challenge that we faced is just there was NaN (Not a Number) in the dataset.

We hope this app someday can track users' happiness so we can use it to predict personalized customized users' happiness/trigger lists. Human emotions are fluctuating, so if ML can detect users' extreme mood changes, it will be a great help for therapists giving diagnoses (if any) easier. So in the future, we can combine CBT therapy and ABCDE therapy so the app can understand the users first before any therapist, hopefully.
