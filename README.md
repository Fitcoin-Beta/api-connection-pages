# Web Page connections

Over here we can see the web pages onces our users perform a task with the API Service. 

The API Service will be downloading the webpages as a simple string, where the API Service will replace certian parameters such as users details and which tracker is connected. 

The idea of having the connection pages being hosted on github is to relieve the API Server's load. Such as css files and other dependencies which are required by the web-site. 

The only web-pages which are being hosted on the services are the OAuth2 service login and Whoop login.
This is because the OAuth2 services needs to be hosted within the micro-service to securly handle the user's login information.
The Whoop login is hosted in the service because Whoop offically do not offer a API Service, so the handling of data of their login will be handled by the service.
The service will send the customised web-pages as a simple string which is then processed automatically by the user's web-browser.