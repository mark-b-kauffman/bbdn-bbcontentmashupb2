ABBCONTENTMASHUP B2
=====================

This project is based from the Spring Tool Suite (STS) Spring MVC project. We've added a bb-manifest.xml and an example of a view that uses the Blackboard Tags to render a page that has the look and feel of other Blackboard Learn pages.
We're building this on top of the Logback B2 to demonstrate placing content using the Build Content Mashup Menu.
Lastly, we've added code that uses the Logback Java APIs to create log files.

Credit to Shane Argo @ All the Ducks for the b2-logging-utils. Thank you Shane!
https://github.com/AllTheDucks/b2-logging-utils

Credit to Scott Hurrey for all the assistance getting this project to pre-compile JSP pages and insert them in the .war file.

### Clone to local repo
####github:
git clone https://github.com/mark-b-kauffman/bbdn-bbcontentmashupb2.git bbdn-bbcontentmashupb2

### Building
To build the project, just run:

./gradlew build

### Deploying
To deploy the B2 to your Learn server, run:

./gradlew -Dserver=host:port deployB2

Example: ./gradlew -Dserver=localhost:9876 deployB2

Home URL Example: `https://<hostname>/webapps/bbdn-abbcontentmashupb2-BBLEARN/`

Continual Logging URL Example: `https://<hostname>/webapps/bbdn-abbcontentmashupb2-BBLEARN/logbacklog`
