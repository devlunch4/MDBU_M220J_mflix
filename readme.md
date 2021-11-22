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

> ## Ticket1: Database Connection
* ### Testing and Running the Application 
    * <pre> mvn test -Dtest=ConnectionTest</pre>
    * <pre> mvn spring-boot:run</pre>
   
    * Q: After passing the relevant tests, what is the validation code for Connection?
      * A: 5a9026003a466d5ac6497a9d


# Chapter 1: Driver Setup

> ## Ticket2: Projection
* ### Testing and Running the Application
    * <pre> mvn test -Dtest=ProjectionTest</pre>
    * <pre> mvn spring-boot:run</pre>

    * Q: After passing the relevant unit tests, what is the validation code for Projection?
        * A: 5a94762f949291c47fa6474d

    
> ## Ticket3: Subfield Text Search
* ### Testing and Running the Application
    * <pre> mvn test -Dtest=TextAndSubfieldTest</pre>
    * <pre> mvn spring-boot:run</pre>

    * Q: After passing the relevant tests, what is the validation code for Text and Subfield Search?
        * A: 5a96a6a29c453a40d04922cc


# Chapter 2: User-Facing Backend

> ## Ticket4: Faceted Search
* ### Testing and Running the Application
    * <pre> mvn test -Dtest=FacetedSearchTest</pre>
    * <pre> mvn spring-boot:run</pre>

    * Q: After passing the relevant tests, what is the validation code for Text and Subfield Search?
        * A: 5aa7d3948adcc3fb770f06fb
