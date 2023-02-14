# Mailer-Microservice

# How to Request

1. Create a form and convert the submission into a JSON or set the enctype to multipart/form-data for the form itself. 
2. Required form fields and their IDs are: Name (name), Email (email), Subject (subject), and Message (message).
3. In a separate JS file, collect the form data into an object and define a function with .addEventListener for the form "submit" button, use FormData on the form-object to convert it into key-value pairs that can be sent with http methods, and then call a send-mail function (also passing it the new FormData object). 
4. The send-mail function may use Fetch() and this url "http://localhost:5000/send" to send the mail object to the microservice.

Example Call: <p>
![image](https://user-images.githubusercontent.com/91649994/218626497-b9b9b0a5-ae56-477a-88a9-60065fb5c7ed.png)
  
# How to Receive

1. After using fetch() in the send-mail function, you may use .then to catch the response.

# UML Sequence Diagram

![image](https://user-images.githubusercontent.com/91649994/218625910-bc0a9cc1-75bd-405a-a632-6373f331922f.png)
