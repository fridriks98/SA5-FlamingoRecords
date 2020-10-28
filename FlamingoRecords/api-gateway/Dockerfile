FROM mcr.microsoft.com/dotnet/core/sdk:3.1

LABEL maintainer="Friðrik Snær Ómarsson"

WORKDIR /app
COPY . /app

ENV ASPNETCORE_URLS=http://+:7000 

RUN dotnet restore
RUN dotnet build

EXPOSE 7000
ENTRYPOINT [ "dotnet", "run"]