FROM mcr.microsoft.com/dotnet/core/sdk:2.2
LABEL maintainer="Arna, Gabriel, Nanna"

WORKDIR /app/customer-service

COPY . /app

RUN dotnet restore
RUN dotnet build

ENV POSTGRES_DB customer_db
ENV POSTGRES_PASSWORD Abc.12345
ENV ASPNETCORE_URLS http://*:80

ENTRYPOINT ["dotnet", "run"]