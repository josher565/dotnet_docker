# dotnet docker from nothin

## dotnet images

https://docs.microsoft.com/en-us/dotnet/architecture/microservices/net-core-net-framework-containers/official-net-docker-images

## How to get a dotnet app hosted in a container

https://docs.docker.com/engine/examples/dotnetcore/

2021-3-17 - currently only dotnet 3.1 is available for docker images, but dotnet 5.0 sdk is out

## Localhost Testing
if you don't have dotnet locally run:
`choco install dotnetcore`
this assumes you have chocolatey installed.. it makes life easier and keeps ur fingers on the kb ;)

```bash
dotnet run
curl -X GET -k https://localhost:5001/weatherforecast
```

## Build & Start the Container

``` bash
docker build -t doc_raw .
docker run -d -p 8080:80 --name doc_raw
curl -X GET http://localhost:8080/weatherforecast
```

## Find & Stop the Container

``` bash
docker ps #find the name
docker stop container_name
```
