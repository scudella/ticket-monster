# ticket-monster
My follow-up on jboss-developer ticket-monster

This is the Building The User UI Using HTML5

We’ve just implemented the business services of our application, and exposed them through RESTful endpoints. Now we need to implement a flexible user interface that can be easily used with both desktop and mobile clients.

See the README under demo.

------------------------------------

We now need to define the services that implement the business logic of the application and expose them to the front-end.

This is the "Building The Business Services With JAX-RS" branch working in Red Hat 8. See part IV of the ticket-monster pdf document.

The "Building the Persistence layer with JPA2 and Bean Validation is in the branch data model. See part III of the ticket-monster pdf document.

The Introduction & Get Started branch is in the branch intro. See part II of the ticket-monster pdf document.

See the README under demo.

---------------------------------
We now have a working data model for the TicketMonster application.

This is the "Building the Persistence layer with JPA2 and Bean Validation. See part III of the ticket-monster pdf document.

---------------------------------

This is the Introduction & Get Started branch working in Red Hat 8. See part II of the ticket-monster pdf document.

On evolution, you may run it as "Run on Server" (Jboss EAD) and check the page http://localhost:8080/ticket-monster/mobile.html. You are supposed to deploy h2-console.war first. See the Deployment section of the document in that part.

The pom.xml has been updated to be able to run the Arquillian test presented in this phase. Arquillian is introduced later in the tutorial. Just right click the test and select "Run as JUnit". You may need to set Maven->Select Maven Profile first.

You can also try:

$ mvn clean test -Parq-wildfly-remote

after starting Jboss server, or 

$ mvn clean test -Parq-wildfly-managed
