FROM mcr.microsoft.com/dotnet/core/sdk:2.2
LABEL maintainer="Arna, Gabriel, Nanna"

WORKDIR /app

COPY . /app
RUN dotnet restore
RUN dotnet build

ENTRYPOINT ["dotnet", "run"]