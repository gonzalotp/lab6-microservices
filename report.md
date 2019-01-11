#### 1: The two microservices are running and registered

* Account microservice running:
![Image 1](report-images/terminal_microservice_account.PNG)
![Image 2](report-images/browser_microservice_account.PNG)

* Web microservice running:
![Image 3](report-images/terminal_microservice_web.PNG)
![Image 4](report-images/browser_microservice_web.PNG)

#### 2: The service registration service has the two microservices registered
* Registration microservice GUI with 2 microservices registered:
![Image 5](report-images/browser_eureka_2registered.PNG)

#### 3: A second account microservice is running on port 4444 and it is registered
* Account microservice running on port 4444:
![Image 6](report-images/terminal_microservice_account_4444.PNG)

* New account microservice registered:
![Image 7](report-images/browser_eureka_4444registered.PNG)

#### 4: What happens when you kill the microservice with port 2222?. Can the web service provide information about the accounts? Why?

When the first account microservice is killed, the web service is still able to provide information about the accounts 
because it makes use of the new account microservice running on port 4444.

The image below shows a log of the new account microservice mentioned, being the last few lines related to the request sent 
by the web microservice.
![Image 8](report-images/terminal_microservice_account_4444_select.PNG)
