# ticket-monster
My follow-up on jboss-developer ticket-monster

This is the Introduction & Get Started branch working in Red Hat 8. See part II of the ticket-monster pdf document.

On evolution, you may run it as "Run on Server" (Jboss EAD) and check the page http://localhost:8080/ticket-monster/mobile.html. You are supposed to deploy h2-console.war first. See the Deployment section of the document in that part.

The pom.xml has been updated to be able to run the Arquillian test presented in this phase. Arquillian is introduced later in the tutorial. Just right click the test and select "Run as JUnit". You may need to set Maven->Select Maven Profile first.

You can also try:

$ mvn clean test -Parq-wildfly-remote

after starting Jboss server, or 

$ mvn clean test -Parq-wildfly-managed
