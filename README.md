![SonarQUbe](https://sonarcloud.io/api/project_badges/measure?project=netcore-lab&metric=alert_status)

# netcore-lab

For my learning .NET CORE 2

## Create Database
Import file *.sql (exclude from GIT)

## RUN as Development
``ASPNETCORE_ENVIRONMENT=Development dotnet run``

## Get Token to access API
Request Token Endpoint: http://localhost:5001/api/token

Send JSON Data

``
{
	"Username": "iFew",
	"Password": "1234"
}
``

Example Return

``
{
    "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE1MTY4MTM0ODgsImlzcyI6Imh0dHA6Ly9sb2NhbGhvc3Q6NTAwMS8iLCJhdWQiOiJodHRwOi8vbG9jYWxob3N0OjUwMDEvIn0.Px5vkJovQLNWd3C-RjOhXJSbqL9Opnxg5jSEmlfZetE"
}
``

## Access API via Token
Using Authorize in Header

Header Example to access to http://localhost:5001/api/member/test

``
Authorization Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE1MTY4MTM0ODgsImlzcyI6Imh0dHA6Ly9sb2NhbGhvc3Q6NTAwMS8iLCJhdWQiOiJodHRwOi8vbG9jYWxob3N0OjUwMDEvIn0.Px5vkJovQLNWd3C-RjOhXJSbqL9Opnxg5jSEmlfZetE
``
