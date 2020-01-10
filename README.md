# Demo-IS
generic demo of WSO2 IS

## Prerequisites

Install WSO2 IS 5.9.0
Install Tomcat 8
Salesforce account
Facebook developer account and Facebook app
Twilio account

## Pre Tasks

### Deploy saml2-web-app-pickup-dispatch webapp and saml2-web-app-pickup-manager webapp and configure IS accordingly
Follow the istructions here: https://is.docs.wso2.com/en/5.9.0/learn/deploying-the-sample-app/#deploying-the-saml2-web-app-pickup-dispatch-webapp

### Define Facebook as Identity Provider
sample parameters:

Clientid: 421682952091284

Client secret: 12344545454

Scope: public_profile,email

User Information field: first_name,last_name,email

Callback url: https://localhost:9443/commonauth

### Define Twilio as Identity Provider
sample parameters:

SMSUrl: https://api.twilio.com/2010-04-01/Accounts/ACd5fbf6a3f8fa1aea3a2e6b0ed2ec459e/SMS/Messages.json

HTTPMethods:POST

HTTPHeader: Authorization: Basic QUNkNWZiZjZhM2Y4ZmExYWVhM2EyZTZiMGVkMmVjNDU5ZTozYmViZTczY2I2OWI0ZmFlOTA2MGE5MWZhMTFjYjdkNw==

HTTP Payload: Body=$ctx.msg&To=$ctx.num&From=%2B15713844564


