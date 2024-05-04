'''

# Intent Classification with LSTM

## Overview
This project demonstrates intent classification using LSTM (Long Short-Term Memory) neural networks. Intent classification is a fundamental task in natural language understanding (NLU), where the goal is to classify text inputs into predefined categories or intents. The project utilizes a dataset containing text samples labeled with different intents, preprocesses the text data, trains an LSTM model for intent classification, and provides a function to predict intents with confidence scores for new text inputs.

## Requirements
- Python 3.x
- TensorFlow
- Keras
- scikit-learn
- NLTK

Install the required libraries using the following command:
```
pip install tensorflow keras scikit-learn nltk
```

## Usage
1. **Data Preparation**: Prepare dataset with text samples labeled with corresponding intents. Ensure the dataset is preprocessed and cleaned.
2. **Data Loading**: Load the dataset into a pandas DataFrame. Ensure it has columns named 'text' for text samples and 'intent' for corresponding intents.
3. **Model Training**: Train the LSTM model for intent classification using the provided notebook or script. The model will be saved as 'best_model.h5'.
4. **Predictions**: Use the trained model to predict intents with confidence scores for new text inputs. You can utilize the provided function `predict_intent_with_confidence`.

## File Descriptions
- `Task 02 NLU Model.ipynb`: Jupyter Notebook containing the code for training the LSTM model.
- `data.text`: Sample dataset containing text samples labeled with intents.
- `best_model.h5`: Trained LSTM model saved after training.

## Functionality
- **Data Preprocessing**: The text data is preprocessed to lowercase, remove punctuation, and tokenize the text samples.
- **Model Architecture**: The model architecture consists of an embedding layer, bidirectional LSTM layers, and dense layers for intent classification.
- **Model Training**: The model is trained using the Adam optimizer and sparse categorical cross-entropy loss function. Learning rate scheduler and model checkpointing are utilized for improved performance.
- **Prediction**: The trained model can predict intents with confidence scores for new text inputs using the `predict_intent_with_confidence` function.


## License
This project is licensed under the [MIT License](LICENSE).

--- 

Feel free to customize this README file according to your project's specific details and requirements.
