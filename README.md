# OpenCloud
**A cloud service providing platform.**

Now everything can be done using cloud computation. From photo, programming, video editing to gaming, creating files in the cloud. Most of these services have a central server which used to do most of the work. But what if we can use every single computer from home computers to server computers to use as servers for those specific computations? That was our main target. But unfortunately for lack of our technical knowledge or resources we are just able to provide only just jupyter notebook service. Which is an open-source web application that allows to create and share documents that contain live code, equations, visualizations and narrative text Our goal is to make every pc as a server for different cloud computation. But in this software we have just used a jupyter notebook as a service and any pc with a dedicated ip address as a server.


**Interface**

Home

![image](https://user-images.githubusercontent.com/78086376/221812402-cbc6caf4-e2d1-4654-8ced-604aa374b261.png)

Packages

![image](https://user-images.githubusercontent.com/78086376/221812515-a38e39a0-3244-4f54-9394-1eb854cf5236.png)

My project section

![image](https://user-images.githubusercontent.com/78086376/221812621-037c9245-61cc-4c6b-a45a-b23ddf934ff6.png)

Registration

![image](https://user-images.githubusercontent.com/78086376/221812723-4ab112a7-b985-4632-8a8d-b226306a68e9.png)

login

![image](https://user-images.githubusercontent.com/78086376/221812782-24341205-854f-435f-bd0a-8d301d5bf268.png)

 Admin panel
 
![image](https://user-images.githubusercontent.com/78086376/221812901-9f4c07dc-e25b-44d9-bb27-cca5bfe0b87f.png)

Session data

![image](https://user-images.githubusercontent.com/78086376/221812974-7aa6cdbb-a4a9-4b2b-824b-222cfa03c0ae.png)


In this project we are trying to develop a web based software. Which will allow to use personal computers or  any computers as servers. For our case it will be a jupyter notebook server . If any one wants to rent their pc as a server they can simply do that by following our process.

![image](https://user-images.githubusercontent.com/78086376/221822242-68137cbd-133a-4c2a-80a8-af29d64c9866.png)

Clients can use Jupyter Notebook from their browser without installing a jupyter server in their computer.  Users can pay with an automatic payment gateway and can use the service instantly. Users can create their projects  and continue their work from anywhere in the world.

The whole system is built using web API technology. We have used ASP.NET core for building the API. The user interface will communicate with the back end using api. Bootstrap, Java Script, HTML and CSS is  used to develop the User Interface. C# is used in  ASP.NET core for building the web API. For communicating with the database there are some custom made classes and functions that have been created. For passing data between the web API to the database or to the front end we need classes. For our database we have used mysql database.

![image](https://user-images.githubusercontent.com/78086376/221822722-f4cad19a-b433-4169-bdce-56c145b3edcc.png)

For saving users/clients password securely we have used hmac protocol for hashing the password. Which will encrypt the password and custom database methods will save it to the users table with all other necessary information.

![image](https://user-images.githubusercontent.com/78086376/221823065-312661a1-6f25-4215-ba2f-2f8200dff7ba.png)


Host/Server computers need to run the application server after entering the key into the appsetting.json file under “HostKey”. Then the Management server will detect that computer as a server for the whole system or network. So when one user clicks to open a project the management server will choose one of the servers available and connect it to the user.  We have used a secret key for verifying the host and client. There will be a session_id for that specific session to start. The project_id will  select the exact project the user wants to work on.

![image](https://user-images.githubusercontent.com/78086376/221823563-d099dba7-5d23-4b5b-8748-6d388b835975.png)


To reduce connecting and disconnecting overhead a connection pooling mechanism has been implemented. The connection pool maintains some steady connections to the database all the time. When a new request is received it picks up a connection from the pool and puts it back when the work is done.

![image](https://user-images.githubusercontent.com/78086376/221823728-1297afbe-e603-4b07-94ff-a332a525da7d.png)





