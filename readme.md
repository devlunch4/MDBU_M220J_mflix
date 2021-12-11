# Chapter 0: Introduction and Setup

> ## README: Setting Up mflix

* ### down m220/mflix-java.zip
* https://s3.amazonaws.com/edu-downloads.10gen.com/M220J/2021/October/static/handouts/m220/mflix-java.zip
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
      mvn -Dtest=&lt;TestClass&gt; test</pre>
    * <pre>cd mflix
      mvn -Dtest=ConnectionTest test</pre>

# Chapter 0: Introduction and Setup

> ## Ticket1: Database Connection
* ### Testing and Running the Application 
    * <pre> mvn test -Dtest=ConnectionTest</pre>
    * <pre> mvn spring-boot:run</pre>
    >* Q: After passing the relevant tests, what is the validation code for Connection?
    >* A: 5a9026003a466d5ac6497a9d


# Chapter 1: Driver Setup

> ## Ticket2: Projection
* ### Testing and Running the Application
    * <pre> mvn test -Dtest=ProjectionTest</pre>
    * <pre> mvn spring-boot:run</pre>
    >* Q: After passing the relevant unit tests, what is the validation code for Projection?
    >* A: 5a94762f949291c47fa6474d


> ## Ticket3: Subfield Text Search
* ### Testing and Running the Application
    * <pre> mvn test -Dtest=TextAndSubfieldTest</pre>
    * <pre> mvn spring-boot:run</pre>
  >* Q: After passing the relevant tests, what is the validation code for Text and Subfield Search?
  >* A: 5a96a6a29c453a40d04922cc 


# Chapter 2: User-Facing Backend

> ## Ticket4: Faceted Search
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=FacetedSearchTest</pre>
  * <pre> mvn spring-boot:run</pre>
  >* Q: After passing the relevant tests, what is the validation code for Faceted Search?
  >* A: 5aa7d3948adcc3fb770f06fb 

> ## Ticket5: Paging
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=PagingTest</pre>
  * <pre> mvn spring-boot:run</pre>
  >* Q: After passing the relevant tests, what is the validation code for Paging?
  >* A: 5a9824d057adff467fb1f526

> ## Ticket6: User Management
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=UserTest</pre>
  * <pre> mvn spring-boot:run</pre>
  >* Q: After passing the relevant tests, what is the validation code for User Management?
  >* A: 5a8d8ee2f9588ca2701894be

> ## Ticket7: Durable Writes

  >* A:   
      WriteConcern.W2
      WriteConcern.MAJORITY

> ## Ticket8: User Preferences
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=UserPreferencesTest</pre>
  * <pre> mvn spring-boot:run</pre>
  >* Q: After passing the relevant tests, what is the validation code for User Preferences?
  >* A: 5aabe31503ac76bc4f73e267

> ## Ticket9: Get Comments
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=GetCommentsTest</pre>
  * <pre> mvn spring-boot:run</pre>
  >* Q: After passing the relevant tests, what is the validation code for Get Comments?  
Hint: We need to sort the comments in the $lookup stage.  
  >* A: 5ab5094fb526e43b570e4633

> ## Ticket10: Create/Update Comments
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=UpdateCreateCommentTest</pre>
  * <pre> mvn spring-boot:run</pre>
  >* Q: After passing the relevant unit tests, what is the validation code for Create/Update Comments?
  >* A: 5aba8d5113910c25d7058f8f