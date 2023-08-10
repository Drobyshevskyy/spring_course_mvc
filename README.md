<h2>Overview</h2>
<br>
A simple web application that allows the first page to link to a second page that requires certain employee data to be entered. This page validates data such as email, phone number, salary, name and surname. Besides the usual textboxes, the page also has radiobuttons and checkboxes to enter some data. After successfully entering all the data and clicking on the "ok" button, we move to the third page, where the application displays on the screen all the information we have entered 
<br>
<br>
Go to the first page by "/", to the second page by "/askDetails", to the third page by "/showDetails"
<br>
<br>
The "first-view.jsp" is responsible for displaying the first page, "ask-emp-details-view.jsp" - for the second page, "show-emp-details-view.jsp" - for the third page
<br>
<br>
Class "MyController.java" is responsible for switching views. All employee fields, getters and setters are described in "Employee.java"
<br>
<br>
Validation of such fields as name, surname, salary and phone number is done by already existing annotations
<br>
<br>
Validation of email is done by annotation written by us; "CheckEmail.java" and "CheckEmailValidator.java" are responsible for this validation
<h3>Configuration</h3>
Project is created from Maven archetype "maven-archetype-webapp"
<br>
Deployment to the server is performed by Tomcat
<br>
DispatcherServlet is configured by file web.xml (/src/main/webapp/WEB-INF/web.xml)
<br>
Spring Container is configured by file applicationContext.xml (/src/main/webapp/WEB-INF/applicationContext.xml)
<br>
<br>
