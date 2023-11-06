# Ex-04_RESTful_Web_Services
## Aim:

To create, deploy and execute RESTful Web service programs using Server, Client and Client-Side remote invocation
## Procedure:

### Server side:
Step 1: Create a new Java Web Project. Follow Steps 1-5 as in SOAP Based Web Service.
Step 2: Right-click on the project name and select New->RESTful Web Services from Patterns.
![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/2ea3b973-3872-42fb-b61e-9e61b8074246)




Step 3: A new window will appear. Select “Simple Root Resource” and click Next.
 ![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/05ad456c-c416-494f-9c3a-95abcba54374)

 


Step 4: In the next window, give a Resource Package name and choose MIME Type as “text/html”. Click Finish.
![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/a4edf9a4-c03f-4f95-8cfa-14651a5473e8)


Step 5: Two editing tabs will appear. Close “ApplicationConfig.java”. You need to write all your required functionalities in GenericResource.java.
Step 6: Alter getHtml() method as shown below.
Step 7: Save your project, clean and build it. Deploy your project.
 ![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/6498aae9-fd9b-4fcf-b29b-f5b91f02b507)


 


Step 8: To test your web service, open a new browser window/tab and type the URL as http://localhost:8080/project_name/webresources/generic?params=45&params=35 and hit enter. (This is the easiest way of testing the web service when it makes use of List).



Client-Side:


Step 1: Create a new Java Web Project. Follow steps 1-5 as in section 1.1.
Step 2: Right-click on the project and select New->RESTful Java Client.
![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/76eecd2a-ea9a-41c1-bc57-123a4cf038d4)




Step 3: A new window will appear. In that, give a name to your client, a package name and select “From Project” under the “Select the REST resource:” tab and click Browse. Step 4: Carefully select your RESTful resource (web service) and click OK.
 ![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/13ee9c45-7920-4a5b-a961-9efe030b03b6)

 


Step 5: Once everything is filled, the New RESTful Java Client window should look like this. Click Finish.
![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/f67c878b-a26a-4ea7-abbb-a46b1732ba74)


Step 6: An editing tab will open. Alter getHtml() method with the following.
![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/ddff1060-3764-44f8-9dc9-2c96247187f9)
 
 


Step 7: Right-click on the Libraries folder under your project and select “Add JAR/Folder”.
![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/db3ec624-b1dc-4c22-aec2-efc22f5a3c5f)


Step 8: A new window will appear. Navigate to the folder where you have placed the “javax.ws.rs-api2.0.1.jar” file and select Open.
 ![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/566218a4-7206-4d7e-af60-0509a5eb492e)

 


Step 9: Right-click on the Web Pages folder and select JSP. In the new window, give a name to the JSP page and click Finish.
Step 10: A new tab will appear with the default contents of the JSP page. In that, include at the top and type the following code to invoke the client java code.
![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/67c1d296-2ac3-4d00-a109-dd9622300af6)


Step 11: Save the project and build it.
Step 12: Run the JSP file and you should see the output in a new browser window.
![image](https://github.com/AjaysuryaS/Ex-04_RESTful_Web_Services/assets/114158396/4d4b4b82-471a-4de8-a80d-ac62dfe61e73)
 
 


Client-Side Remote Invocation:


Step 1: Follow steps 1-5 as in Section 2.2
Step 2: In the generated NewJerseyClient.java file, Replace BASE_URI from private static final String BASE_URI = "http://localhost:8080/RESTful_Server/webresources"; TO private static final String BASE_URI = "http://192.168.116.62:8080/RESTful_Server/webresources";
Step 3: Follow steps 6-12 as in Section 2.2


## Result:
 Thus, the RESTful web service program has been successfully created and executed.
