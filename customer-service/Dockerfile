FROM mcr.microsoft.com/dotnet/core/sdk:2.2
LABEL maintainer="Arna, Gabriel, Nanna"

WORKDIR /app/customer-service

ADD ../customer-db/db-scripts/init.sql /app
COPY . /app

RUN dotnet restore
RUN dotnet build

ENV ASPNETCORE_URLS http://*:80

ENTRYPOINT ["dotnet", "run"]