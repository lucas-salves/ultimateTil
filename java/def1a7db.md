# Containers

## Java EE Servers
Server application that provides the standard EE services. Sometimes caled application servers, because allow you to serve application data to the clients, much like web servers serve web pages to browsers.
An example of Java EE Server is Tomcat.
There are two types of servers: application servers and web servers. The following items are application server examples:
* JBoss: open-source from JBoss community
* Glassfish: provided by Sun Microsystem, now acquired by Oracle.
* Weblogic: Provided by Oracle
* Websphere: Provided by IBM.
Applcation servers are used to host services for end users.

## Java EE Containers
The interface between the component and the lower-level functionality that supports EJB,JMS, JTA and other Java EE APIs.

## The web container / Servlet Container
The interface between web components (servlets, JavaServer Face Facelets page, or a JSP page) and the web server.The web container manages the component's lifecycle, dispatches requests to respective servlets and provides information about the current request.

## Applications Client Container
The interface between Java EE application clients. Clients are Java SE applications that uses Java EE server components, and the Java EE server. It runs on the client machine and is the gateway between the client application and the Java EE server components that the client uses.

## EJB Container
The interface between enterprise beans that provides the business logic.
It handles transaction management and security authorization and allows a bean developer to concentrate on the business issues.

### References

- [Enterprise JavaBeans EJB](https://www.techopedia.com/definition/443/enterprise-javabeans-ejb)
- [Recipient Web](https://pt.wikipedia.org/wiki/Recipiente_web)
- [Java Containers](https://docs.oracle.com/javaee/6/firstcup/doc/gcrkq.html)
- [Java EE application server](https://quick-adviser.com/what-is-java-ee-application-server/)
