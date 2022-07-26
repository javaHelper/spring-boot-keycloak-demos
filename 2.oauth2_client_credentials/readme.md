# OAuth2 Client Credentials:

<img width="1090" alt="Screenshot 2022-07-26 at 4 50 20 PM" src="https://user-images.githubusercontent.com/54174687/180994152-d5718f89-80df-47cf-bbf9-9fe797dc1037.png">

<img width="872" alt="Screenshot 2022-07-26 at 4 43 20 PM" src="https://user-images.githubusercontent.com/54174687/180993174-510d6f18-f869-492c-860f-4b7b1666947f.png">

<img width="858" alt="Screenshot 2022-07-26 at 4 43 44 PM" src="https://user-images.githubusercontent.com/54174687/180993190-1be1e0d5-a1f4-4a12-9832-f715e2148565.png">

---

- Grant Type: Client Credentials
- Access Token URL: http://localhost:8080/realms/oauth2-demo-realm/protocol/openid-connect/token
- Client ID: oauth2-client-credentials
- Client Secret: 3QKnwiNLUqt4LQG3WGUzyy5EFphc4UUq
- Scope: openid


<img width="888" alt="Screenshot 2022-07-26 at 4 49 16 PM" src="https://user-images.githubusercontent.com/54174687/180993979-59769058-01a0-4d53-b97c-8e68459dc5af.png">

GET ->

```sh
curl --location --request GET 'http://localhost:8083/microservice1/home/webclient' \
--header 'Authorization: Bearer eyJhbGciOiJSUzI1NiIsInR5cCIgOiAiSldUIiwia2lkIiA6ICJxWGdUZ3FwTnV1aDYzdWVWQWE0aGIzYUkyYWlGNnFLcGdCMGdZNWFDN3I4In0.eyJleHAiOjE2NTg4MzM3OTgsImlhdCI6MTY1ODgzMzQ5OCwianRpIjoiYzdkNmRjNzgtMDAwYS00NWUzLWIwNWMtZmUzY2ExNjIyNjE0IiwiaXNzIjoiaHR0cDovL2xvY2FsaG9zdDo4MDgwL3JlYWxtcy9vYXV0aDItZGVtby1yZWFsbSIsImF1ZCI6ImFjY291bnQiLCJzdWIiOiI5YTIwZWIxZi1jMjQwLTRkOTMtODExMC1mYzFhYmRkNTkxY2IiLCJ0eXAiOiJCZWFyZXIiLCJhenAiOiJvYXV0aDItY2xpZW50LWNyZWRlbnRpYWxzIiwiYWNyIjoiMSIsInJlYWxtX2FjY2VzcyI6eyJyb2xlcyI6WyJvZmZsaW5lX2FjY2VzcyIsInVtYV9hdXRob3JpemF0aW9uIiwiZGVmYXVsdC1yb2xlcy1vYXV0aDItZGVtby1yZWFsbSJdfSwicmVzb3VyY2VfYWNjZXNzIjp7ImFjY291bnQiOnsicm9sZXMiOlsibWFuYWdlLWFjY291bnQiLCJtYW5hZ2UtYWNjb3VudC1saW5rcyIsInZpZXctcHJvZmlsZSJdfX0sInNjb3BlIjoib3BlbmlkIHByb2ZpbGUgZW1haWwiLCJjbGllbnRIb3N0IjoiMTcyLjE3LjAuMSIsImNsaWVudElkIjoib2F1dGgyLWNsaWVudC1jcmVkZW50aWFscyIsImVtYWlsX3ZlcmlmaWVkIjpmYWxzZSwicHJlZmVycmVkX3VzZXJuYW1lIjoic2VydmljZS1hY2NvdW50LW9hdXRoMi1jbGllbnQtY3JlZGVudGlhbHMiLCJjbGllbnRBZGRyZXNzIjoiMTcyLjE3LjAuMSJ9.E_bbNAZDKT-l9eeZCEFzVb-OuVfQJiwQY9Jf1NnsrpYQ18fO__kP7Kh--c6HYKjFFGI2C1gtaXNIFBAqabmzMxJ1cPSDd_10mWArVSzCCEnVykpXseeVRn7qgsz-JQ0QGvSXN92EeDxp0EspSxH4G4LSyI9or3LHmVX4i6mdxsi2ExfRPJw8YVC7b-9SIZ97R6A_3It0joYBG_fajiWQmarRm9wser6ff3YBpyrHm31kH4jn4wAil_WQg-OL2IGi4999VWMTMcTy9SaveV4WMzpkVvscr7QekLa6SM0yWMF5jcSP5JZJDqHOtZ4ffWn8JumniFlNH_C_aIqANPhUWw' \
--header 'Cookie: JSESSIONID=F3978A05C8315B430A6159B61219FC09'
```
