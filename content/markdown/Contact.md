Add content below to the file as shown in canvas

<B> GETTING STARTED</B> <br>

  Content experience API (Application Program Interface) provides the ability for 3rd party applications to connect to the medanco system in order to retrieve inventory data. This api have  1 resources and is POST requests.

This API uses the HTTP Authorization header to pass authentication information to all end points. The Authorization header has the following format.<br>


POST: https://{domain_name}/{application_name}/api/v1/  


<p>
   client_id      ############ <br>
   client_secret  ############ <br>
   caller_id      ############ <br>
</p>


<p>Details of how to obtain your Client ID, Client Secret are given below in the "Security" section. <br></p>

**Unauthorized Access**

<P>If the Client ID and Client Secret are invalid the following HTTP Response will be returned.<br> </p>
<p>
HTTPS/1.1 401 Unauthorized <br>
Server: API Gateway/1.3.2 <br>
Content-Type: application/x-www-form-urlencoded <br>
Date: Wed, 14 Jul 2017 21:11:51 EST <br>
X-MULE_ENCODING: US-ASCII <br>
Content-Length: 34 <br>
Invalid client_id or client_secret
</p>



**Endpoints**

 - Finally, details of all of the API endpoints can be found in “Endpoints”.

**Using the APIs to fetch response**

 - Open any REST-test client application, for instance Chrome Postman
   or, SOAP UI
 - Put the resource URL in a URL tab, along with required parameters (if applicable)
 - Provide {client_id,} and {client_secret,} as key-value pairs through add header section.
 - Select the request access method, for example, GET/POST
 - Send the request

**Security**

 **Requesting API Access**

 - After signing in to the Developer Portal, you will need to register
   your application to generate your Client ID and Client secret (its
   mandatory you have pass this details).
 - From the Exchange homepage, click on the specific API that you wish to work with.
 - Click on &quot;Request API access&quot;, &quot;New application&quot;.
 - Fill in the form with details of your application.
 - Click Add.
 - Now, select the Standard SLA Tier and review the Terms and Conditions.
 - Click Request API Access again and your application will then be created.
- Your Client ID and Client secret can be found by clicking on &quot;My applications&quot; from the Exchange Portal homepage.