# Neural Network SMS Text Classifier 📱💬

## Project Overview
This project focuses on developing a neural network model to classify SMS messages as either "ham" (normal messages) or "spam" (advertisements or unwanted messages). The classifier will predict the probability of each message being spam, providing a useful tool for filtering unwanted messages.

## Challenge Description
The task is to implement a function, `predict_message`, that:
1. Takes a string input representing an SMS message.
2. Returns a list with:
   - A probability score between **0** and **1** indicating how likely it is for the message to be "ham" (0) or "spam" (1).
   - A label ("ham" or "spam") based on the predicted score.

## Dataset
The **SMS Spam Collection dataset** is used for this project. It contains SMS messages labeled as either "ham" or "spam." The dataset is pre-split into training and testing sets to streamline model development and evaluation.

## Key Steps
1. **Data Preparation**: Load, clean, and preprocess the text data to make it compatible with a neural network model.
2. **Model Building**: Construct a neural network, ideally with TensorFlow or Keras, optimized for text classification tasks.
3. **Model Training**: Train the network on the SMS Spam Collection dataset, allowing it to learn patterns that distinguish spam from ham messages.
4. **Implement `predict_message`**: The function will take raw message text as input, process it, and use the trained model to predict whether it’s "ham" or "spam."

## Sample `predict_message` Function
```python
def predict_message(message):
    # Preprocess the input message
    processed_message = preprocess(message)
    # Make prediction with the trained model
    prediction = model.predict(processed_message)
    # Determine label based on prediction score
    label = "spam" if prediction > 0.5 else "ham"
    return [prediction[0], label]
