# Spam Email Classification

This project focuses on building machine learning models to classify emails as either "ham" (not spam) or "spam".

## Dataset

The dataset used in this project is the [Spam Email Classification dataset](https://www.kaggle.com/datasets/ashfakyeafi/spam-email-classification) from Kaggle. It contains a collection of emails labeled as either 'ham' or 'spam'.

## Project Steps

The following steps were taken in this project:

1.  **Data Loading and Exploration**:
    *   The dataset was downloaded from Kaggle using `kagglehub`.
    *   The data was loaded into a pandas DataFrame.
    *   Initial exploration was performed to understand the data structure, columns, and identify any potential issues (like the unexpected category entry).

2.  **Data Preprocessing and Cleaning**:
    *   The unexpected category entry in the 'Category' column was identified and removed to ensure data integrity.
    *   The dataset was balanced by downsampling the 'ham' messages to match the number of 'spam' messages.
    *   Text cleaning steps were applied to the 'Message' column, including:
        *   Removing the word 'subject'.
        *   Removing punctuation.
        *   Removing stop words.

3.  **Data Visualization**:
    *   Count plots were generated to visualize the distribution of 'ham' and 'spam' emails before and after balancing.
    *   Word clouds were generated for both 'ham' and 'spam' emails to visualize the most frequent words in each category.

4.  **Model Development**:
    *   **LSTM Model**: An LSTM model was built for classification. The text data was tokenized and padded to a fixed length. The model architecture included an Embedding layer, an LSTM layer, and Dense layers. Early stopping and ReduceLROnPlateau callbacks were used during training.
    *   **Naive Bayes Model**: A Multinomial Naive Bayes model was also implemented. The text data was vectorized using TF-IDF (Term Frequency-Inverse Document Frequency).

5.  **Model Training and Evaluation**:
    *   Both the LSTM and Naive Bayes models were trained on the prepared training data.
    *   The models were evaluated on the test data using metrics such as accuracy, classification report, and confusion matrix.

## Results

*(You can add specific results here after running your models. For example:)*

*   The Naive Bayes model achieved an accuracy of [Your Naive Bayes Accuracy]% on the test set.
*   The LSTM model achieved an accuracy of [Your LSTM Accuracy]% on the test set.

*(Discuss the performance of each model and any insights you gained.)*

## Technologies Used

*   Python
*   pandas
*   numpy
*   matplotlib
*   seaborn
*   nltk
*   tensorflow (for LSTM)
*   sklearn (for Naive Bayes and data splitting/evaluation)
*   kagglehub

## How to Run the Code

1.  Clone this repository.
2.  Make sure you have the necessary libraries installed (you can use `pip install -r requirements.txt` if you create a requirements file).
3.  Download the dataset using `kagglehub.dataset_download("ashfakyeafi/spam-email-classification")`.
4.  Run the Jupyter Notebook cells sequentially.


