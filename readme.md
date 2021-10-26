# Chapter 0: Introduction and Setup

> ## README: Setting Up mflix

* ### down m220/mflix-java.zip
* ### Local Environment Dependencies
    * Java 1.8
    * Maven

* ### Running the Application
    * "mflix/src/main/resources" directory you can find a file called "application.properties".
        * spring.mongodb.uri=mongodb+srv://m220student:m220password@<YOUR_CLUSTER_URI>
    * <pre>cd mflix
      mvn spring-boot:run</pre>
    * And then point your browser to http://localhost:5000/.

* ### Running the Unit Tests
    * <pre>cd mflix
      mvn -Dtest=<TestClass> test</pre>
    * <pre>cd mflix
      mvn -Dtest=ConnectionTest test</pre>

# Chapter 0: Introduction and Setup

> ## Ticket: Database Connection
* ### Testing and Running the Application 
    * <pre> mvn test -Dtest=ConnectionTest</pre>
    * <pre> mvn spring-boot:run</pre>
   
    * Q: After passing the relevant tests, what is the validation code for Connection?
      * A: 5a9026003a466d5ac6497a9d

