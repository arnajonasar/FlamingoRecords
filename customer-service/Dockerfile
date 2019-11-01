FROM mcr.microsoft.com/dotnet/core/sdk:2.2
LABEL maintainer="Arna, Gabriel, Nanna"

WORKDIR /app/customer-service

COPY . /app
WORKDIR /app/customer-service

RUN dotnet restore
RUN dotnet build

ENV ASPNETCORE_URLS http://*:80

ARG POSTGRES_PASSWORD
ARG POSTGRES_DB

VOLUME [ "/${PWD}/customer-db/db-scripts:/docker-entrypoint-initdb.d postgres" ]

ENTRYPOINT ["dotnet", "run"]