# dotnet docker from nothin

## dotnet images

https://docs.microsoft.com/en-us/dotnet/architecture/microservices/net-core-net-framework-containers/official-net-docker-images

## Image names & purpose

Image	Comments
mcr.microsoft.com/dotnet/aspnet:5.0	ASP.NET Core, with runtime only and ASP.NET Core optimizations, on Linux and Windows (multi-arch)
mcr.microsoft.com/dotnet/sdk:5.0	.NET 5, with SDKs included, on Linux and Windows (multi-arch)

We'll use the chunky one that's easy to get code with: mcr.microsoft.com/dotnet/sdk:5.0

## docker file:

https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/docker/building-net-docker-images?view=aspnetcore-5.0

## URLs

https://localhost:5001/swagger

https://localhost:5001/weatherforecast

## Commands

``` bash
docker build -t doc_raw .
```
