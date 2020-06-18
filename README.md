# Postman API test challenge
<h2>Prerequisites</h2>

* Install Postman

<h2>API Information</h2>

* Request Type - POST (URL is different per environment
* Authorization - Bearer Token (different per environment)
* Headers - Key:Content-Type | Value:application/json
* Body Type - JSON/raw (see json_body_format in repo)
* Required Information
  * firstname
  * crmKey

<h3>Stage Information</h3>

* Authoriziation Bearer token & CRM Key - YzczNWNmZDItM2JmYy00OTNiLTk2YzgtOGFiOWZhMGQ0MzViM2ZkMGEzMGMtYmI1ZC00Y2RhLWFjZmQtNDRhZGQyNjc0MDU1
* POST URL - https://stage-api.acculynx.com/api/v1/leads/import-homeadvisor-lead/

<h3>Production Information</h3>

* Authoriziation Bearer token & CRM Key - MTQxNmY1ZjktYTM1MC00ZjI4LTgxZWItMzZhNmM5NGQxNmEwMmVkYWQ3YzQtYjQ1Ny00Mjk2LWIwOGYtOTA0OWVlZTA3ODZj
* POST URL - https://api.acculynx.com/api/v1/leads/import-homeadvisor-lead/

<h2>API Test Challenge</h2>

For this testing challenge, you will be creating a Postman collection with three tests to verify an API call.
1. Verify that a successful call returns a 202 code and takes less than 1000 ms to run.
2. Verify that when first name is not added, an error occurs.  Verify the error message that returns is "The firstName field is required."
3. Create a test that will always fail. An example would be expecting a 202 code for a request missing a first name.

* Tests should be written in a way that can be ran against Stage and Production by using variables for data that changes per environment.
* Tests should be able to be executed in the Postman Runner. There should be 2 passes and 1 fail.
