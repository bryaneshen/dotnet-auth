# dotnet-auth
Learning how to secure a .NET CORE API with JWT Bearer authentication.

Use case of our application:
![image](https://user-images.githubusercontent.com/47930778/231011373-121c7398-8f5e-4d2f-ae50-859699e6c76d.png)
The client will first request to acquire a token from Azure. Assuming the client is authorized to acquire a token, it will then be received from Azure. When the client makes an HTTP request to the API, it will send the token along with its request. 
The API will check (with the help of Azure) that the token is valid, it will return back a HTTP response.
