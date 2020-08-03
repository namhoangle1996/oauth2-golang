## Go OAuth example

In order to run the application:

1. Method : GET [http://localhost:9096/credentials] . You will get a client ID and client secret.
2. Replace the values of the `clientID` and `clientSecret` variables in this link :
```http request
http://localhost:9096/token?grant_type=client_credentials&client_id=f3c11b45&client_secret=26c16768&scope=read&access_token_exp=20
```
   :+1: You will get this if valid {"access_token":"53NUK3XHNEIB0JJSFXHQ1Q","expires_in":7200,"scope":"read","token_type":"Bearer"} 

3.Method : GET [http://localhost:9096/protected?access_token=53NUK3XHNEIB0JJSFXHQ1Q] with access_token got above
  
  Or with header : 
  ```text
    Authorization : Bearer 53NUK3XHNEIB0JJSFXHQ1Q
```

# oauth2-golang

