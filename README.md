## Project set up

An example of a project with all we need to start a professional project.

In this project we will be addressing:

- Code structure (Component structure)
- Configuration
- Multi module
- Multi environments 
- Quality assurance (Sonar)
- Database migrations (Liquibase)
- Infrastructure as a code


Details:
- Using Mvn profile to handle different environments
- Using mvn multi modules
- Using Maven revision to handle version from the outside `mvn package -Drevision=42.1`
- Using Maven to generate the Docker image
- Creating a third party library to be used across  different projects, 
with no dependency attached to it and with a conditional to load the configuration only if a specific dependency 
is present in the project
- Setting all properties in the Core module and only overwriting in the Web module
- Ensuring code quality using Sonarcobe 
- Managing database changes using Liquibase
- Structuring the code using the Component pattern
- Managing the structure using Docker and Kubernates
- Managing logs with logback
