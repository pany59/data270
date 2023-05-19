# DATA 270 Project
#  SMS Spam Detection with Natural Language Processing

Yuan Pan, Johnny Qiu, Lu Yang, Manyu Zhang

Department of Applied Data Science, San Jose State University

Data 270: Data Analytics Processing

Dr. Eduardo Chan

May 19, 2023

***
## Abstract
With the development of communication technology, short message service (SMS) has become an important part of people's daily life. However, cheap and easy to send spam was then prevalent and had many negative effects. Therefore, it is urgent to develop and improve the technology to obtain effective and reliable detection and interception of spam. The main objective of this project is to achieve accurate and reliable spam detection based on natural language processing (NLP) technology.

For effective supervised machine learning, the Ling-Spam corpus from The Linguist List, a prominent online resource for academic linguistic research, was selected as the dataset. This resource consists of four directories representing the states of stop-word processing. In each directory, the data is divided into 10 subdirectories, which each contain 289 individual messages saved as text files, and they have been classified by professionals, such as "spmsg" for spam in the file name.

In this project, only the raw data under the "bare" directory was used for data processing. Then by using Python to read all the files in the directory and convert them into a 2893 row Pandas dataframe, which includes three columns of data: "label" "subject" and "main body". Next, data cleaning was then performed, including handling of incomplete and missing data, handling of noisy data, and handling of inconsistent data. In addition, data transformation was performed to remove Stop Words and transform the text in "main_body" into a high-dimensional vector by TF-IDF method and Bag of Words method. After the transformation, TruncatedSVD was used to reduce the dimensionality of the two datasets obtained from different transformation methods, and the datasets were then divided into training, validation, and testing datasets in a ratio of 0.6, 0.2, and 0.2, respectively.
