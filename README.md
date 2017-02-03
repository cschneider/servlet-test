# Example for issue

[https://ops4j1.jira.com/browse/PAXWEB-1060]

# Build

mvn clean install

# Install

Start karaf 4.1.0

```
feature:install http-whiteboard scr 
install -s mvn:net.lr/servlet-test/1.0-SNAPSHOT
service:list Servlet
http:list
```

The service should be exported. http:list only shows the servlet if only one property is present.

# Test

[http://localhost:8181/test]
