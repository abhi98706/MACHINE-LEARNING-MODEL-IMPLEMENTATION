# MACHINE-LEARNING-MODEL-IMPLEMENTATION

*NAME*: ABHIJIT DAS

*INTERN ID*: CT06DR1737

*DOMAIN*: PYTHON PROGRAMMING

*DURATION*: 6 WEEKS

*MENTOR*: NEELA SANTOSH

## DESCRIPTION

Spam detection is an important application of machine learning that focuses on identifying unwanted, irrelevant, or potentially harmful messages. In this project, the goal is to build a simple yet effective predictive model capable of classifying email messages as either “spam” or “ham” (non-spam). This type of binary classification is widely used in email services, messaging systems, and cybersecurity applications to filter harmful content, prevent phishing attacks, and reduce digital clutter. The entire task is carried out using the Python programming language, which is popular in the field of data science due to its readability, flexibility, and the availability of powerful machine-learning libraries.

The first step in the process is the creation or collection of a dataset that contains email texts along with corresponding labels. Each message is tagged as “spam” if it contains characteristics commonly found in malicious or promotional emails, or “ham” if the message is normal and safe. In many projects, large public datasets such as the Enron email dataset or SMS spam datasets are used. However, for demonstration purposes, a small sample dataset may also be constructed manually. This dataset is handled using the pandas library, a core Python tool that simplifies the process of loading, storing, and manipulating tabular data. Pandas helps structure the data into a DataFrame, making it easier to clean, view, and preprocess the text before applying machine-learning techniques.

Emails consist of unstructured text, which cannot be directly used as input for machine-learning models. Therefore, the next stage involves converting the textual data into a numerical format. This is where the feature extraction step comes into play. In this project, the transformation is performed using TfidfVectorizer from the scikit-learn library. TF-IDF stands for Term Frequency–Inverse Document Frequency. It is a widely used technique that measures how important a word is within a document relative to all the documents in the dataset. Words that appear frequently in a message but rarely in other messages are given higher importance. This helps the model distinguish between general and spam-indicative words. For example, terms like “win”, “free”, “urgent”, or “click here” often receive higher weights in spam messages.

Once the textual data is transformed into numerical vectors, the dataset is divided into training and testing subsets using scikit-learn’s train_test_split function. The training set is used to teach the machine-learning model how to differentiate between spam and ham, while the test set is used to evaluate how well the model performs on new, unseen messages.

The chosen model for this task is Logistic Regression, implemented through scikit-learn’s LogisticRegression class. Although the name suggests a regression technique, Logistic Regression is actually a powerful algorithm for binary classification tasks. It works by estimating the probability that a message belongs to the spam category based on the extracted features. Logistic Regression is widely preferred for its simplicity, efficiency, and strong performance on text-classification problems.

After training, the model is ready to make predictions. When new email messages are passed through the same TF-IDF transformation and then fed into the model, it outputs either “spam” or “ham”. In this version of the project, the focus is strictly on producing the classification results, without printing accuracy scores, confusion matrices, or other evaluation metrics. The output simply displays each message from the test set along with its predicted label.

In summary, this project demonstrates how machine learning can be applied to text-based email classification using Python, pandas, scikit-learn, and TfidfVectorizer. It showcases the complete workflow—from data preparation, feature extraction, and model training to final prediction—providing a foundational understanding of how spam detection systems operate in real-world applications.

## OUTPUT

<img width="693" height="423" alt="Image" src="https://github.com/user-attachments/assets/82ac0d16-7597-4283-be17-080b02ba9812" />
