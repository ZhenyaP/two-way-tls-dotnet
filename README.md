# two-way-tls-dotnet
The sample dockerized ASP.NET Core application with mutual (two-way) TLS negotiation.
--------------------------------------------------------------------
For simplicity (for demo purposes), self-signed root CA cert 
is used for issuing server and client certificates.

For client authorization, X.509 client certificates are used.
NGINX proxy server is used for the following purposes:
- client authorization;
- load balancing;
- SSL/TLS termination

The application is dockerized (Dockerfile and docker-compose.yml are included).