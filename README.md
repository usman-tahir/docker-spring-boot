# docker-spring-boot
Basic setup for a Docker image with Spring Boot

### Overview
The `build.gradle` file has a basic setup for building a Spring Boot application. It manages the dependencies needed for the application, and allows you to add plugins based on your project setup. Once you run `gradle build`, a gradle daemon is started, and installs/configures the listed dependencies (if it is your first time running the application), and gives you a `BUILD SUCCESSFUL` or `BUILD FAILED` status, which provides ample feedback to diagnose any problems, should you encounter the latter.

### Setting up the Spring Boot Application locally
Once you've cloned this repository into your local environment, make sure that the correct Java version is set based on your environment, and then make sure that any additional plugins that you may require (Eclipse, iDEA, etc.) have been added.

Then, from the root directory of this project, run the following:

`gradle build && java -jar build/libs/gs-spring-boot-docker-0.1.0.jar`

Once the application sends back a `BUILD SUCCESSFUL` log message, navigate to `localhost:8080` to see your application run and display the default message for the route setup in `Application.java`.

