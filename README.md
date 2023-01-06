# Spam-Filter

In recent years, internet has been created several platforms for making human life become more secure. Among these; e-mail is a substantial platform for user communication. Email is nothing; simply it’s called an electronic messaging framework which transmits the message from one user to another.
Nowadays, e-mail has turned into a typical medium because of its several branches like Yahoo mail, Gmail, Outlook etc., which are completely free for all web user by following some administration . At present, Email called a secure worldwide communication medium for its several functions. But sometimes email becomes more hazardous for some “Spam Email”.
Generally, Spam email called as junk email or unsolicited message which sent by spammer through Email. The process is, collected the address on the web and sends the message through domain's username. Actually, it has been produced for financial profits using I the assortment of procedures and instruments that incorporate spoofing, bonnets, open intermediaries, mail transfers, bulk mail instruments called mailers, and so forth. Spam filtering is a challenging undertaking for an assortment of reasons. For spam email, users are facing several problems like abuse of traffic, limit the storage space, computational power, become a barrier for finding the additional email, waste users time and also threat for user security. So, becoming email more secure and effective, appropriate Email filtering is essential.
Spam filtering is a process to detect unsolicited massage and prevent from entering into user’s inbox. Now days, various systems have been existed to generate anti-spam technique for preventing unsolicited bulk email. Most of the anti-spam methods have some inconsistency between false negatives (missed spam) and false positives (rejecting good emails) which act as a barrier for most of the system to make successful antispam system. Therefore, an intelligent and effective spam-filtering system is the prime demand for web users.

 ## System Design
 
 Artificial neural networks are widely used to solve a large number of problems in various spheres of human activity. Due to its universal approximating ability, neural network models are used in solving problems such as diagnostics, control, forecasting, pattern recognition, etc. However, neural networks were most famous in solving classification problems.
On the Fig below we can see the scheme of the neural network technology application for e-mail classification.

 ![image](https://user-images.githubusercontent.com/66063140/211050399-ffcee5b7-676a-4139-8a27-49c7dcbfea64.png)

## Approach

• Artificial neural network structure selection (number of inputs, outputs, hidden layers and neurons in each hidden layer);
• Artificial neural network training with using training set ("spam"/"not spam" e-mail messages); 
• using artificial neural network for e-mails classification. The artificial neural network can accurately classify spam messages and recognize new types of spam in e-mails. The trained neural network’s weights contain information about the spam e-mails that determines the efficiency of this technology application.

The artificial neural network filtration model construction involves the following steps:
• obtaining the initial e-mail messages data, including examples of "spam" and "not spam" messages;
• Initial data pre-processing and training sample forming;
• Artificial neural network structure development: inputs, outputs, number of layers and neurons in each layer;
• Artificial neural network training for spam filtration model construction;
• Artificial neural network spam filtration model testing and evaluation.
At unsatisfactory results of the evaluation model, we need to go back to one of the steps and perform all the steps in the given order. Choice of the initial phase is determined experimentally.
It is necessary for the analysis to pre-select significant parameters from the original text information. Then the values of the selected parameters will enter the training set.
Email Spam Filtering using Neural Networks
The result of e-mails classification depends on the following message attributes:
• Frequency of the words in uppercase;
• Frequency of the numbers in the message;
• Number of different colors;
• Size of the message text;
• Number of blank lines.
Then we use mathematical statistics methods to evaluate the attribute’s informativity.
These initial data are presented in a tabular form, where each row corresponds to a single letter, and each column represents different letter features. The values of particular email message attributes are shown in the cells of the table.
Then it is necessary to pre-treat data in the table. The table can contain parameters having the same value for the whole column. These attributes can not individualize objects being studied. So they must be excluded from the analysis. Also table may contain some categorical attribute values which all records are different. Clearly this field cannot be used for data analysis and should be deleted.
At the same time while cleaning the data on the table columns (attributes), we also pretreat data on the table rows (records). Any real database typically contains errors and not well-defined values (corresponding to some rare or exceptional situations) and other defects that can reduce the effectiveness of spam filtering. These records must be deleted, because they are not statistically significant.

## TESTING AND RESULTS

TESTING THE SYSTEM AND DISCUSSING THE RESULTS The result of the artificial neural network training is the email messages classification model. The model adequacy can be evaluated by contingency table showing the results of the classification on the original data from the training data set.

![image](https://user-images.githubusercontent.com/66063140/211050153-9adb99bf-1fad-42b5-bec1-6d6f36122487.png)

As this table shows, 17 of the 500 e-mails were classified incorrectly, i.e. general error of the model was 3.4%. The error of the 1st kind (erroneous skipping of spam) was found to be0.8%, and the error of the 2nd kind (erroneous detection of spam) was 5.9%. In order to evaluate the neural network model generalization capability, we built contingency table showing the results of the testing data set classification.

![image](https://user-images.githubusercontent.com/66063140/211050215-fc8d469e-d4a6-4b80-944c-7f07361931dc.png)

As the table shows, 5 of the 500 e-mails were classified incorrectly, i.e. general error of the model was 2.5%. The error of the 1st kind (erroneous skipping of spam) was found to b1%, and the error of the 2nd kind (erroneous detection of spam) was 4%. The experimental studies have shown that developed artificial neural network model is adequate and it can be effectively used for the e-mail messages classification, for example, in intelligent spam filtering system.
