# Academic-Query-Classification
To resolve students' doubts we need to understand the doubt category. Based on the category we can serve the best result for the asked query
# Overview
Embibe, a leading educational platform, is collaborating with Kaggle to launch an exciting AI competition focused on academic text classification. This competition aims to revolutionize how Embibe understands student intent and query types, ultimately providing more precise and valuable results to its users.

Challenge Objective: The competition challenges data scientists and AI enthusiasts to create innovative models for classifying academic text, focusing on students' queries and intents.

Real-world Impact: Improving Embibe's understanding of student needs will lead to personalized and accurate content recommendations, enhancing the learning experience for millions of students.

Diverse Data: Participants will work with a diverse dataset comprising academic text, student queries, and user interactions, enabling them to build robust and adaptable models.

Problem Complexity: Participants will face the complexities of natural language processing (NLP) as they tackle the nuances of academic language, query types, and user intentions.

Evaluation Metrics: Submissions will be evaluated based on precision, recall, F1-score, and other relevant NLP metrics, ensuring a comprehensive assessment of model performance.

Benefits: Participants who will develop cutting-edge solutions to this problem will get a chance to work at Embibe.

Skill Development: Aspiring data scientists can enhance their NLP skills and gain valuable experience while working on a problem with direct societal impact.

# Description
The task at hand involves the classification of academic queries into multiple predefined categories, which include 'academic_servable', 'academic_non_servable', 'general', 'junk', and 'conversational'. The goal is to assign each query to its most appropriate category accurately. However, it's important to note that the training dataset for this task exhibits class imbalance, which means that some categories may have significantly fewer examples compared to others.

# Objective 
The goal of this task is to build a machine learning or natural language processing model that can accurately classify academic queries into predefined categories based on their content and intent.

# Evaluation
The primary evaluation metric for this task is accuracy, which measures the proportion of correctly classified queries among all queries in the dataset.

# Dataset Description
Files
train.csv - the training set
test.csv - the test set
sample_submission.csv - a sample submission file in the correct format

# Columns
unique ID query_text category
unique ID - Unique ID corresponding to the query text
query_text - query text
category - category of the query

# Details of the classification classes (categories):
academic_servable: Queries that indicate a clear intent to seek or provide academic services, such as tutoring, research assistance, or course-related help. e.g. 'what is inertia'.
academic_non_servable: Queries related to academic topics but without a clear intent to seek or provide services. These might include general academic discussions or queries about educational concepts. e.g. 'What will come in place of the question mark(?) in the given number series?'.
general: Non-academic queries that cover a wide range of topics unrelated to academics. e.g. 'Could you give me a brief overview of haryana police si'.
junk: Queries that contain irrelevant, nonsensical, or spam content. e.g. 'X-Men: Mutant Academy 2'.
conversational: Queries that are part of a conversation or dialogue and don't necessarily fall into the other categories. e.g. 'ansar me'.

# Note
Training Dataset contains a total of 5k query texts and their categories tagged.
Training data has an imbalance.

# Save final submission
Suppose your final data frame is output. Save the final output to the file 'submission.csv' containing only two columns 'unique ID' and 'category'.
output[['unique ID', 'category']].to_csv('submission.csv', index=False)
Then after saving the notebook version submit the output for evaluation.
