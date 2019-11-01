FROM mcr.microsoft.com/dotnet/core/sdk:2.2

LABEL "author"="Eyþór"

USER root

ENV ASPNETCORE_URLS=http://+:7000
ENV ASPNETCORE_ENVIRONMENT=Production

ADD . /app

WORKDIR /app

RUN dotnet restore

ENTRYPOINT dotnet run