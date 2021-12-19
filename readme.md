

20211218 END. but Need ReView Course or ReStart Course.

find connect error..


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

> ## Ticket11: Delete Comments
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=DeleteCommentTest</pre>
  * <pre> mvn spring-boot:run</pre>
  >* Q: After passing the relevant tests, what is the validation code for Delete Comments?
  >* A: 5ac25c280a80ed6e67e1cecb


# Chapter 3: Admin Backend

> ## Ticket12: User Report
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=UserReportTest</pre>
  * <pre> mvn spring-boot:run</pre>
>* Q: After passing the relevant tests, what is the validation code for User Report?
>* A: 5accad3272455e5db79e4dad

> ## Ticket13: Migration
* ### Testing and Running the Application
  * <pre> mvn clean compile exec:java -Dexec.mainClass="mflix.Migrator"</pre>
  * <pre> mvn test -Dtest=MigrationTest</pre>
  * <pre> mvn spring-boot:run</pre>
>* Q: After passing the relevant tests, what is the validation code for Migration?
>* A: 5ad9f6a64fec134d116fb06f

# Chapter 4: Resiliency

> ## Ticket14: Connection Pooling
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=ConnectionPoolingTest</pre>
  * <pre> mvn spring-boot:run</pre>
>* Q: After passing the relevant tests, what is the validation code for Connection Pooling?
>* A: 5ad4f4f58d4b377bcf55d742

> ## Ticket15: Handling Timeouts
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=TimeoutsTest</pre>
  * <pre> mvn spring-boot:run</pre>
>* Q: After passing the relevant tests, what is the validation code for Connection Pooling?
>* A: 5addf035498efdeb55e90b01

> ## Ticket16: Error Handling
* ### Testing and Running the Application
  * <pre> mvn test -Dtest=HandlingErrorsTest</pre>
  * <pre> mvn spring-boot:run</pre>
>* Q: After passing the relevant tests, what is the validation code for Error Handling?
>* A: 5ae9b76a703c7c603202ef22
