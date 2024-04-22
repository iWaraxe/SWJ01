# Introduction to Selenium WebDriver(Java) course.
## Task 000. Preparing for the training
Read Rules of training before start.
Please install:
- Java SDK ([Open JDK 21 version](https://jdk.java.net/archive/)) 
- [IntelliJ IDEA Community Edition](https://www.jetbrains.com/idea/download/?section=windows#section=windows). 
- [Install Maven](https://maven.apache.org/download.cgi). 
- Install Mozilla Firefox and Google Chrome browsers and​ [Geckodriver](https://github.com/mozilla/geckodriver/releases)​ + [​Chromedriver​](https://googlechromelabs.github.io/chrome-for-testing/) for them.​


## Task 005. Video - What is unit testing?
​Please, watch introduction [video](https://coherentsolutions.sharepoint.com/sites/training-center/_layouts/15/stream.aspx?id=%2Fsites%2Ftraining%2Dcenter%2FPrograms%2FTest%20Automation%2Fvideo%2Fen%2FIntro%2Emp4&ga=1)


## Task 010. Unit testing. JUnit
JUnit is a unit-testing framework. JUnit 5 ​is the next generation of JUnit, it includes the best from all existing unit-testing frameworks. [JUnit 5 wiki](https://junit.org/junit5/docs/current/user-guide/) provides a detailed description of the framework. 
Download the project and refer to the wiki page - complete Task 10, described in the document below.


### Task Conditions
**Do not change the code of the application.**
The project contains a piece of internet-shop. Each user has a cart, which contains items(products). 
Each cart can be stored in JSON format, and then you can load the cart from a JSON file. A simple example of usage is placed in src/main/java/Main. 
All test classes that you are going to create should be placed in src/test/java.


1. Develop unit tests for the JsonParser class (one of them should be an Exception test with >= 5 datasets). Determine by yourself, how many tests should be developed
2. Develop 1 test for RealItem class
3. Develop 1 test for VirtualItem class
4. Develop 2 tests for the Cart class
5. Disable one of the tests from point 1
6. Add grouped assertion for one of the tests(*)


Tests should be grouped into different categories. Usage of Before/After annotations is required. Use the latest version of JUnit 5. After the code review, we will have a meeting in Teams, where you will explain why you decided to write exactly these tests but not others.


### Task Rubric for Grading Unit testing. JUnit


#### Proficiency Levels RUBRIC
1. **Basic**
   - **Criteria**: Adheres strictly to the task requirements with no additional tests. Uses `Before/After` annotations correctly and employs the latest version of JUnit 5. All tests are logically placed in the correct directory.
   - **Evaluation**: Completion of the exact number of tests as specified in the task (5 tests including the disabled one, with grouped assertions where indicated).


2. **Advanced**
   - **Criteria**: Goes beyond the basic requirements by creating more tests than specified. These additional tests should cover significant functionalities not explicitly mentioned in the task but are crucial for ensuring the robustness of the code under test.
   - **Evaluation**: Number of tests exceeds the task requirements. Quality and relevance of the additional tests are considered.


3. **Expert**
   - **Criteria**: All tests from the "Advanced" level plus ensuring high quality and real need for each test. Tests should avoid redundancy, have clear purposes, and cover edge cases effectively.
   - **Evaluation**: High average quality rank across all tests, with each test demonstrating clear value in testing critical and edge case functionalities.


4. **Guru**
   - **Criteria**: Identifies and highlights flaws or issues in the provided codebase through testing. This level requires a deep understanding of potential bugs, edge cases, and failure modes.
   - **Evaluation**: Number and significance of identified issues through testing. Tests should not only pass or fail but must also effectively demonstrate the presence of bugs or design flaws.


5. **Impossible**
   - **Criteria**: Not only identifies issues as in the "Guru" level but also suggests and implements code changes that resolve these issues. This level requires modifying the application code to fix identified problems, demonstrating a profound understanding of both the testing framework and the application under test.
   - **Evaluation**: Quality and effectiveness of code changes in addressing the identified issues. Tests should pass consistently after modifications, proving the issues have been resolved.


#### Test Quality Evaluation Metric
P = (Num/MinRN) * (AveQR/MaxQR)^w = (Num * AveQR^2)/125
Where:
- Num is the total number of tests written, normalized against the minimum required number of tests.
- MinRN is the minimum required number of tests. In case of JUnit task trainee needs to write at least 5 tests. So in the formula RQ equals to 5.
- AveQR is the average quality rank of the tests on a 5-star scale, with the quality rank itself also being squared to emphasize its weight.
- MaxQR is the maximum quality rank, in our case maximum quality rank is 5 stars.
- w is the weight. In our case is equal to 2.


This formula ensures that while both the quantity and the quality of tests contribute to the final parameter P, the quality (as reflected by the w=2) plays a more significant role, and its impact is normalized to keep the scale balanced.


To grade an assignment, firstly I will define the proficiency level of the task completion: basic, advanced, expert, guru, or impossible, and then calculate the quality evaluation metric using formula.
