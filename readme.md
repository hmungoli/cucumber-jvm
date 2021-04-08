# Component Tests Overview
* Component tests are developed to test the middleware logic to process and route the requests from TPS to downstream system and vice versa.
* Tests are run on the dev envrionment where the middleware is neither connected to downstream nor TPS, so tests depends on the mock service 
  for the response.
* Tests rely on Elastic Search where the service logs the payload which is validated with the expected payload in the tests.

# Instructions for running the Component Tests:

**Prerequisites**

*  Mock services should be created individually for each service and should be deployed in the apass environment.
*  Mock service and actual service should be up before running the tests.

# How to run tests via Jenkins
*  Navigate to Jenkins jobs [component tests](https://docs.oracle.com/javase/10/install/installation-jdk-and-jre-macos.htm)

*  Click on Build with Parameters.

*  Select Service and Group and click on Build.

*  After completion of the build Citrus Report is generated.
