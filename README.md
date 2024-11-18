# sms_spam_detector
 Mod21 challenge
Module 21 Challenge
Due Nov 14 by 11:59pm Points 100 Submitting a text entry box or a website url Attempts 0 Allowed Attempts 4
Background
You'll be refactoring code from an SMS text classification solution into a function that constructs a linear Support Vector Classification (SVC) model. Once the model is created and trained, you will create a Gradio app to host the application, enabling users to test text messages. The application will provide feedback to users, indicating whether the text is classified as spam or not, based on the model's performance.

Files
Download the following files to help you get started:

Module 21 Challenge filesLinks to an external site.

Before You Begin
Before starting the assignment, be sure to complete the following steps:

Create a new repository for this project called sms_spam_detector. Do not add this homework assignment to an existing repository.

Clone the new repository to your computer.

Inside your local Git repository, add the starter files from your file downloads.

Push these changes to GitHub or GitLab.

Challenge Instructions
The starter files consist of the following files: gradio_sms_text_classification.ipynb, sms_text_classification_solution.ipynb, and SMSSpamCollection.csv.

Create the SMS Classification Function
Using the code in the sms_text_classification_solution.ipynb file, create the sms_classification function in the gradio_sms_text_classification.ipynb by doing the following:

Set the features variable to the text message column of the DataFrame.

Set the target variable to the "label" column of the DataFrame.

Split data into training and testing and set the test_size to 33%.

Build a pipeline to transform the test set to compare to the training set.

Fit the model to the transformed training data and return model.

Load the SMSSpamCollection.csv into a DataFrame and call the sms_classification function with the DataFrame, and set the result to the "text_clf" variable.

Create the SMS Prediction Function
Use the sms_prediction function to predict the classification of a new text by doing the following:

Create a variable that will hold the prediction of a new text.

Use a conditional statement that determines if the text message is "ham" or “spam”.

If the message is “ham”, the function should return the following message: f'The text message: "{text}", is not spam.'

If the message is spam, the function should return the following message: f'The text message: "{text}", is spam.'

Create the Gradio Interface Application
Create a Gradio Interface application that takes a textbox for the inputs and has a textbox for the output. The textboxes should have labels that describe what each textbox contains.

Launch the application and provide the URL to share the application. Your application should look like the following:

The SMS prediction Gradio application interface

Use the following text messages to test your application.

1. You are a lucky winner of $5000!
2. You won 2 free tickets to the Super Bowl.
3. You won 2 free tickets to the Super Bowl. Text us to claim your prize.
4. Thanks for registering. Text 4343 to receive free updates on medicare.
Requirements
Create the SMS Classification Function (50 points)
The features variable is set equal to the text message column of the DataFrame. (8 points)

The target variable is set equal to the "label" column of the DataFrame. (8 points)

The data is split into training and testing sets, and the test_size is set to 33%. (8 points)

A Pipeline is built using the TfidfVectorizer and LinearSVC to transform the test set and compare it to the training set. (8 points)

The model is fitted to the transformed training data and the model is returned. (8 points)

The SMSSpamCollection.csv is read into a DataFrame. (5 points)

The DataFrame is passed to the sms_classification function and the result is set equal to the "text_clf" variable. (5 points)

Create the SMS Prediction Function (30 points)
A variable that holds the prediction of a new text is created. (8 points)

A conditional statement that determines if the text message is "ham" or “spam” is created. (12 points)

The conditional returns a message if the text is “ham”. (5 points)

The conditional returns a message if the text is “spam”. (5 points)

Create the Gradio Interface Application (20 points)
A Gradio Interface application is created with three parameters for the “function”, “outputs”, and “inputs”. (6 points)

The “outputs” parameter is a textbox that contains a label to let the user know what to type in the box. (4 points)

The “inputs” parameter is a textbox that contains a label to let the user know that the prediction will be displayed in the textbox. (4 points)

The Interface application can be shared with other users with a public URL. (2 points)

The Gradio Interface works as expected and there are no errors after a user submits a text message. (4 points)

Grading
This assignment will be evaluated against the requirements and assigned a grade according to the following table:

Grade	Points
A (+/-)	90+
B (+/-)	80–89
C (+/-)	70–79
D (+/-)	60–69
F (+/-)	< 60
Submission
To submit your Challenge assignment, click Submit, and then provide the URL of your GitHub repository for grading.

note
You are allowed to miss up to two Challenge assignments and still earn your certificate. If you complete all Challenge assignments, your lowest two grades will be dropped. If you wish to skip this assignment, click Next, and move on to the next module.

Comments are disabled for graded submissions in Bootcamp Spot. If you have questions about your feedback, please notify your instructional staff or your Student Success Manager. If you would like to resubmit your work for an additional review, you can use the Resubmit Assignment button to upload new links. You may resubmit up to three times for a total of four submissions.

important
It is your responsibility to include a note in the README section of your repo specifying code source and its location within your repo. This applies if you have worked with a peer on an assignment, used code that you did not author or create sourced from a forum such as Stack Overflow, or you received code outside of curriculum content from support staff such as an Instructor, TA, Tutor, or Learning Assistant. This will provide visibility to grading staff of your circumstance in order to avoid flagging your work as plagiarized.

If you are struggling with a Challenge assignment or any aspect of the academic curriculum, please remember that there are student support services available for you:

Ask the class Slack channel/peer support.

AskBCS Learning Assistants exists in your class Slack application.

Office hours facilitated by your instructional staff before and after each class session.

Tutoring GuidelinesLinks to an external site. - schedule a tutor session in the Tutor Sessions section of Bootcampspot - Canvas

If the above resources are not applicable and you have a need, please reach out to a member of your instructional team, your Student Success Advisor, or submit a support ticket in the Student Support section of your BCS application.

References
Tiago, A., Hidalgo, J. 2012. SMS Spam Collection. UCI Machine Learning Repository. Available https://archive.ics.uci.edu/dataset/228/sms+spam+collectionLinks to an external site. [2023, October 25]. (CC-BY 4.0Links to an external site.).

