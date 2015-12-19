##1.-First part, Account and Web
### Account Microservice
![Account Microservice](https://raw.github.com/Shathe/Laboratory-6-microservices/master/accounts.jpg)
### WebService Microservice
![WebService Microservice ](https://raw.github.com/Shathe/Laboratory-6-microservices/master/web.jpg)

##2.- Dashboard
![Dashboard](https://raw.github.com/Shathe/Laboratory-6-microservices/master/dashboard.jpg)

##3.- A second account registered
![Account Microservice 2](https://github.com/Shathe/Laboratory-6-microservices/blob/master/dashboard.jpg?raw=true)

##4.- A brief report describing what happens when you kill the first account microservice
When you kill the first account microservice, the web service, can not provide any information about the Account service, (the conecction fail with a "refused connection" error. It happens, because the connection the web is trying to perform is the one using the port 2222 which is no longer avaidable.
Then you can see a "No instances available for ACCOUNTS-SERVICE" message when the service realize the account service is down. Finally, when the web service ask if there is other account service running in some other port, (round 20 secs later) the web services shows the other account service running in the 4444 port with its information. You can see the flow of all this information at the dashboard (only a bit info) and above all in the console logs.
