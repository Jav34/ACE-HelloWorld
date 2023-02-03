# Description

`Hello World` application is a demonstration of the possibilities of working on the IBM ACE bus version 12.0.5. It does not execute business functionality. 

The application returns "Hello World" string to the client in .json format and provides the following endpoint:

**`/acehelloworld/v1:`**

![message flow image](images/flow.png)

Using a *GET* method, it sends a request to the serwer and receives the mentioned string in response. 


# Implementation

**`helloWorld`**

![message flow image](images/flow.png)

The `HTTP Input node receives the request`. The `helloWorld` compute node creates the message tree and message body:

![Alt text](images/compute.png)

 Finally, `HTTP Reply` node sends the message to the client.

 # Format

 The app uses .json 