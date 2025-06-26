# Course 3: Data Science Methodology

This folder contains my final assignment for **Course 3** of the IBM Data Science Professional Certificate on Coursera — *Data Science Methodology*.

## Topic Chosen
**Classifying Emails as Spam or Not Using Text-Based Features**

Spam detection is a classic and practical problem in machine learning. It has real-world importance for both personal productivity and organizational security.

## Data Science Methodology Applied

### **Business Understanding**

#### Problem Statement:
The problem I want to solve is the evergrowing presence of spam Emails in the inbox. They waste time, clutter inboxes and often carry a lot of security problems. Users and organizations need a simple way to filter out all of these annoying mails so that they can focus on what is more important.

#### Data Question:
_Can we classify emails as spam and not spam based on its contents using machine learning?_

This question defines the problem we have to solve and also gives an ideaof what approach we can use to address the solution.

### **Analytic Approach**  
Since the final output we need is a simple "Yes" or "No" we can use a basic classification approach of supervised machine learning. The goal is to train a model that will accurately identify is a mail is spam or not based on the labeled examples given to it in the training stages.

### **Data Requirements**  
We will need a dataset of emails that includes:

- The email body (text)
- Subject line
- Sender information
- Time sent
- A label indicating whether each email is spam or not spam

This will allow us to extract useful features (like word frequency, presence of certain keywords, sender domain, etc.) to train our model.

### **Data Collection**  
  We will use a public datasets like the "Enron Email Dataset" or the "SpamAssassin Corpus", which includes thousands of labeled emails.

### **Data Understanding & Preparation**  
We will:

- Explore the Dataset and figure out if the data collected can help us in answering the problem defined
- Clean the Dataset by addressing missing values, duplicates and any other inconsistencies
- Preprocess the text by removing stopwords, punctuation, and applying tokenization. 
- Extract features for making the data useful in training the model
- Split the data into training and testing sets.

### **Modeling & Evaluation**  
We will build classification models using our training dataset and evaluate their accuracy using multiple metrics like **Accuracy, Recall, Precision and F1-Score**.  A high precision and recall will be especially important for spam detection, since false positives (misclassifying important emails as spam) are costly.

---

No coding was required for this stage — just a complete problem-to-solution blueprint using data science methodology.

