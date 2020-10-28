FROM mcr.microsoft.com/dotnet/core/sdk:3.1

LABEL maintainer="Friðrik Snær Ómarsson"

WORKDIR /app/customer-service
COPY . /app

WORKDIR /app/customer-service

ENV ASPNETCORE_URLS=http://+:80

ARG POSTGRES_PASSWORD
ARG POSTGRES_DB

RUN dotnet restore
RUN dotnet build

ENTRYPOINT [ "dotnet", "run"]