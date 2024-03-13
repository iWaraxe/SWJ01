# Training topics:  
## Rules of the training [https://coherentsolutions.sharepoint.com/:w:/s/training-center/ETVnSKs6hl9MspwFmHZpGiwBhAWeIQccIqm64Kj8oNpFyQ]
1. Unit testing (Junit5, TestNG)  
2. Locators (xpath, css)  
3. Selenium WebDriver (overview, api)  
4. Page object pattern (classic, page factory)  
5. Reporting (Allure)  
6. Cloud services (SauceLabs)  
7. Selenium Grid  
 

## Pre-requisites (points that must be considered for the training): 

1. Knowledge of the basics of working with Git. 
2. Knowledge of the basics of Java programming language. 
3. Availability of free time to work on the training. It is advisable to coordinate this training with your TL or PM so that he/she is aware of such an activity of his/her employee from the project. Do not forget that the training should be done outside of working hours. Sometimes candidates refer to a lack of time due to work on the project, that is why it should be taken into account that the training is a non-project activity, and the time for its fulfillment should be allocated outside of business hours. 

## Information to Web Course 

Training contains 15 different tasks and 4 videos. Each task has a description and materials. A trainee must read and understand all the materials related to the task and then complete all the requirements from the task file. After finishing that, a trainee must set 75% for a particular task as a task progress and open pull request on GitHub or Bitbucket. A link to the pull request must be sent to the trainer via Email or Microsoft Teams. The trainer performs the code review and changes task progress percentage. The trainer sets 100% if everything is okay or the code contains minor mistakes. If the code requires important updates – the trainer can set 85%, 70%, etc. (depending on the number of mistakes). A trainee must update code according to the comments from the code review and then inform his/her trainer that additional code review is required in the scope of the same pull request. 
A trainee is obligated to inform his/her trainer about vacations or other activities, which will stop the training process for 1 week or more. If there are no obstacles, then it is advised to complete at least one task per week (depending on the task scope). If a trainee is assigned to a project, then he/she should work on the training in his/her own time. Training must be completed in < 3 months. If training takes > 3 months, then situation will be reviewed individually (continue or stop the training and find the cause of a slow progress). 
All tasks have the answers inside the materials provided for each task. If a trainee has difficulties, then he/she can ask the trainer for advice or a hint (only about the task itself, not about c# or java/git). The final task is the end of the training. Based on this task the trainer forms feedback for stakeholders, therefore a trainee works on it without any help. 

## Software

1. Please install Java SDK (Open JDK 21 version [https://jdk.java.net/archive/]) and IntelliJ IDEA Community Edition [https://www.jetbrains.com/idea/download/#section=windows].
2. Install Maven [https://maven.apache.org/download.cgi].
3. Install Mozilla Firefox and Google Chrome browsers and​ Geckodriver [https://github.com/mozilla/geckodriver/releases]​ + ​Chromedriver [https://googlechromelabs.github.io/chrome-for-testing/]​ for them.​

## Task 10 Unit Testing (JUnit)
### Introduction video
​Please, watch introduction video: [https://coherentsolutions.sharepoint.com/:v:/s/training-center/ERvr7QT-T5xDgagrTJ4j0IcBbX3YQC3wU4nOFIo5a1Lvyw?e=c0vUqE]

### JUnit
JUnit is a unit-testing framework. JUnit 5 ​is the next generation of JUnit, it includes the best from all existing unit-testing frameworks. JUnit 5 wiki provides a detailed description of the framework. 
JUnit wiki: [http://junit.org/junit5/docs/current/user-guide/]

Download the project and refer to the wiki page - complete Task 10, described in this document.

Do not change the code of the application. 

Project contains a piece of internet-shop. Each user has a cart, which contains items(products).  
Each cart can be stored in JSON format and then you can load the cart from JSON file. Simple example of usage is placed in src/main/java/Main.  
All test classes, which you are going to create, should be placed in src/test/java. 
  
### Task 10: 
1. Develop unit tests for JsonParser class (one of them should be Exception test with >= 5 datasets). Determine by yourself, how many tests should be developed 
2. Develop 1 test for RealItem class 
3. Develop 1 test for VirtualItem class 
4. Develop 2 tests for Cart class 
5. Disable one of tests from point 1 
*6. Add grouped assertion for one of tests   
 
Tests should be grouped into different categories. Usage of Before/After annotations is required. Use the latest version of JUnit 5. After code review, we will have a meeting in Teams, where you will explain why you decided to write exactly these tests, but not others.  
