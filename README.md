This demonstrates the use of sql lite with java / hibernate


1. 
https://www.sqlitetutorial.net/sqlite-java/sqlite-jdbc-driver/

for the jdbc driver

1.1
eventually downloaded jdbc jar file : 
https://jar-download.com/artifacts/org.xerial/sqlite-jdbc/3.27.2.1/source-code 

since added indirection of maven files (use maven to auto download unfortunately).

2. Some tips :
https://www.sqlite.org/java/raw/doc/overview.html?name=0a704f4b7294a3d63e6ea2b612daa3b997c4b5f1

3. the config file is changed : 

		<property name="connection.url">jdbc:sqlite:./test</property>

4. 
org.hibernate.dialect.SQLiteDialect

from : 
https://gist.github.com/rppowell-lasfs/f0e3b2d18c3be03ada38a3e367eaf1b8


5. No user name and password:
https://www.srccodes.com/annotation-based-hibernate-hello-world-example-using-maven-build-tool-and-sqlite-database/

6. add sqllite dialect:

https://jar-download.com/artifacts/net.kemitix/sqlite-dialect/0.1.0/source-code
This did not work.
Instead I had  download the java file & then add it
to the java project. I should be able to add the dialect class file as a jar. (unfortunately the .jar I obtained from above does not have a source code). I obtained the sqllite dialect file from the link in item above (#5).

