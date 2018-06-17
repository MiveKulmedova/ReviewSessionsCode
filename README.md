Running Feature files in paralell using maven plugins:

cucumber-jvm-parallel-plugin:
For each feature file in your project, it will create a separate CukesRunner.

cucumber-jvm-parallel-plugin -> generate runners for each FEATURE,SCENARIO

maven-failsafe plugin -> will take those runners and run them in
paralell

maven-failsafe plugin vs maven-surefire plugin

command to run feature files in paralell:

mvn -Dtest=SomeTests -DfailIfNoTests=false verify

==================================================

Did you ever run Cucumber feature files or scenarios in parallel?

Yes, there are multiple ways to achieve that. The way i did was by using
cucumber-jvm-parallel-plugin along with maven-failsafe plugin. And I also set up
selenium grid in Amazon AWS EC2 machine.

Can you elaborate please?
Sure! The way it works is:
 cucumber-jvm-parallel-plugin will generate a runner class for each feature or scenario
 and store in the project. Then maven-failsafe plugin will pick up those runners
 and execute them in paralell.
 In my code when I instantiate the browser - i use new RemoteWebDriver and point to the
 URL of the hub. and my tests run in Amazon EC2 machine.
 ===========================
 RESTApi automation framework - yes and you are doing it right now in your current project. Not little bit, not in previos projects, Or you just exposed to it.
 Sell them what they need. Of course you can mention your overall skillset.
 -------
 Whenever you are talking about your skills, current role in project
 UI test automation with Selenium Webdriver
 API test automation with RestAssured, Postman etc
 DATABASE test automation SQL, JDBC
 
 ------------
 I run my smoke and regression tests from jenkins in EC2 machine via GRID or i can run locally. 
 









