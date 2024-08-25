# Automated Customer Support Ticket System for Financial Services

In the financial industry, customer complaints are invaluable as they often highlight areas for improvement in products and services. Efficiently addressing these complaints not only reduces customer dissatisfaction but also strengthens customer loyalty and retention. Furthermore, resolving issues swiftly provides insights for continuous service enhancement, helping to attract and retain more customers.

However, customer complaints are typically unstructured text data. Traditionally, companies assign teams of support employees to manually review and route each ticket to the appropriate department. As customer bases grow, this process becomes increasingly tedious and resource-intensive.

This project aims to automate the process of handling customer support tickets using natural language processing (NLP) techniques. The solution will classify and assign tickets to relevant departments—such as credit cards, banking, or mortgages/loans—based on the content of the complaint. This automation will improve response efficiency and allow the company to scale its customer support system more effectively

### Business Goal
The goal of this project is to build a model capable of classifying customer complaints based on the products or services they relate to. By categorizing the tickets accordingly, the system aims to expedite the resolution process, improving customer satisfaction and reducing response times.

Using non-negative matrix factorization (NMF), a topic modeling approach, recurring patterns and key words from the complaint tickets were detected. This method uncovered important features associated with each cluster of categories. By organizing the tickets into clusters, the underlying topics of customer complaints were identified.

The project involved performing topic modeling on the provided .json dataset. Since the data was unlabelled, NMF was applied to detect patterns and classify the tickets into five clusters based on the following products/services:

Credit card / Prepaid card
Bank account services
Theft/Dispute reporting
Mortgages/Loans
Others
Once the topics were identified, a labelled dataset was created to train supervised models, such as logistic regression, decision trees, and random forests, enabling automatic classification of new customer complaints.

### Dataset
The dataset consists of 78,313 customer complaints stored in a .json format, including 22 features. The data was first converted to a dataframe for further processing and analysis. download link: https://drive.google.com/file/d/1O1AO9AI6Y70e2iqTeD8Ma-hOX6IgQ8V4/view

### Tasks Completed
The following eight major tasks were completed to achieve the project goal:

- Data Loading: The .json dataset was loaded and converted into a dataframe for further analysis.

- Text Preprocessing: The raw text data underwent preprocessing, including tokenization, removal of stopwords, stemming/lemmatization, and other cleaning steps to prepare it for analysis.

- Exploratory Data Analysis (EDA): Detailed EDA was performed to gain insights into the distribution and nature of the complaint data.

- Feature Extraction: Key features were extracted from the text data to assist in clustering and classification.

- Topic Modeling: Non-negative matrix factorization (NMF) was applied to identify the underlying topics and segregate the complaint tickets into clusters.

- Model Building using Supervised Learning: Once the clusters/categories were established, the labelled data was used to train supervised models. Three models were trained: logistic regression, naive Bayes, and random forest.

- Model Training and Evaluation: The models were trained and evaluated based on accuracy, precision, recall, and F1-score, allowing for a comparison of their performance.

- Model Inference: The best-performing model was used to classify new customer complaint tickets into their respective categories, streamlining the complaint resolution process.
