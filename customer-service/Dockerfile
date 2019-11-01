FROM mcr.microsoft.com/dotnet/core/sdk:2.2

LABEL "author"="Eyþór"

USER root

ENV ASPNETCORE_URLS=http://+:80

ADD ./customer-service/ /app

WORKDIR /app

RUN dotnet restore

ENTRYPOINT [ "dotnet", "run" ]

FROM postgres

USER postgres

ENV POSTGRES_PASSWORD=Abc.12345
ENV POSTGRES_DB=customer_db

ADD ./customer-db/ /db

WORKDIR /db

CMD [ "./db-scripts/init.sql" ]

