# Lamda functions

## Repo Content
### 1. Lamda-1
> `Description`: A lamda function calling an external API to fetch and serve random cat pictures.

> `Setup`: 
```
1. Create an AWS Lamda function from scratch and paste the given code.
2. Create an AWS API Gateway (HTTP) and add a Resource (e.g: Lamdatest).
3. Create a GET method for the resource and connect the Lamda function of Step 1.
```

> `API Configuration (under the GET method)`:
```
4. Method Response -> under 200, add response header as Content-Type
5. Method Response -> Under 200, delete application/json in Response Body for 200
6. Integration Response -> Under 200 -> Header Mappings -> Change mapping value to 'text/html'
7. Integration Response -> Under 200 -> Mapping Template -> Add Mapping Template as text/html. In the body, add $input.path('$')
8. Deploy the API. (e.g. Create a deploy stage of Dev)
9. Note the API Endpoint from the API Dashboard.
10. Call the API endpoint from your Browser or Postman. e.g- <API Endpoint>/<resourceName>
```

> `E.g. Output Endpoint`:
```
https://fipiwompql.execute-api.us-east-1.amazonaws.com/dev/lamdatest
```
