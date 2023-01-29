# Lab Report 2
The code for StringServer is shown below along with two images of adding strings to the server.

![StringServer](https://user-images.githubusercontent.com/122580017/215230190-6cdd453b-be36-4a0a-a02f-ea8745f16997.png)

The image below demonstrates good morning being added to the StringServer. By adding /add-message?s=Good Morning after the server port, this calls the main method in the class StringServer, which then calls the handleRequest method. The handleRequest method uses localhost:5898/add-messages?s=Good Morning as its argument. By calling handleRequest with the path add-messages?s=Good Morning it changes the instance variable string from " " to "Good Morning" as a result of the if statement on the 19th line. Then after setting the instance variable string to Good Morning it returns the string Good Morning.  
![String1](https://user-images.githubusercontent.com/122580017/215230244-949791b4-769d-48dc-ade5-650aebca4cbd.png)

The image below demonstrates when another string is added to the StringServer. The first method which is called is the main in the class StringServer. Main then calls the method handleRequest which uses localhost:5898/add-messages?s=Hello as its argument. By calling handleRequest with this argument it changes the instance variable string from "Good Morning" to "Good Morning\nHello" which is shown in the 24th line. After the instance variable string is updated it then returns this string, therefore results in the image below. 
![String2](https://user-images.githubusercontent.com/122580017/215230254-4be85352-4f39-49d3-ac48-528831a22adb.png)

