FROM mcr.microsoft.com/dotnet/core/sdk:2.2
LABEL maintainer="Arna, Gabriel, Nanna"

COPY . /app
ADD ../customer-db/db-scripts/init.sql /app
WORKDIR /app/customer-service

RUN dotnet restore
RUN dotnet build

ENV ASPNETCORE_URLS http://*:80

ENTRYPOINT ["dotnet", "run"]