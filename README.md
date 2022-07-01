# Introduction:

Exploratory data analysis popularly known as EDA is a process of performing some initial investigations on the dataset to discover the structure and the content of the given dataset. It is an unavoidable step in the entire journey of data analysis right from the business understanding part to the deployment of the models created.

EDA is where we get the basic understanding of the data in hand which then helps us in the further process of Data Cleaning & Data Preparation.

## Overview:
In this repository I performed EDA on Research Problems: Model to predict the Behavioral Challenges in ASD_Kids(1-18 Years) dataset. This dataset contains the factors involving in developing ASD for children. It consists of: 
1. A10_Autism_Spectrum_Quotient                       
2.  Social_Responsiveness_Scale                         
3.  Age_Years                                            
4.  Qchat_10_Score                                      
5.  Speech Delay/Language Disorder                      
6.  Learning disorder                                   
7.  Genetic_Disorders                                   
8.  Depression                                           
9.  Global developmental delay/intellectual disability  
10.  Social/Behavioural Issues                           
11.  Childhood Autism Rating Scale                        
12.  Anxiety_disorder                                    
13.  Sex                                                
14.  Ethnicity                                          
15.  Jaundice                                             
16. Family_mem_with_ASD                                 
17. Who_completed_the_test                             

## Results and observations:

After performing EDA I have explored different kinds of classification algorithms and compared the results obtained by them. 
The algorithms which I have used and their score after 10Fold stratified split are:
1. Logistic Regression (96.7%)
2. Decision trees(97.34%)
3. Support Vector Machines(99.57%)
4. Adaboost Classifier(95.6%)
5. Random Forest classifier(100%)
6. Gradient Boosting(98.54%)
7. XGboost classifier(98.3%)

We can see that Random Forest Classifier performed the best among all other classification algorithms getting an accuracy of over 100 percentage followed by Kernel Support Vector Machine with accuracy of 99.5%.

Adaboost Classifier and Logistic regression performed the worst among all other algorithms with accuracies of 95.6% and 97.3% respectively.

Other algorithms performed decently with score between(97.3 -98.3)percentage

As Random Forest Classifier starts by taking feature importance and splits into branches, I have observed that through criterion:'entropy' for splitting
Qchat_10_Score feature has got the highest importance and contributes more in deciding the child develops Autism spectrum disorder in future. 
Children with more Qchat_10_Score got more probability in developing ASD_traits. 

