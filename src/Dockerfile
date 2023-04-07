# FROM mcr.microsoft.com/dotnet/sdk:7.0-alpine AS build
# WORKDIR /app

# # copy csproj and restore as distinct layers
# COPY ./src ./
# RUN dotnet restore

# # copy and publish app and libraries
# RUN dotnet publish -c Release -o out


# # Enable globalization and time zones:
# # https://github.com/dotnet/dotnet-docker/blob/main/samples/enable-globalization.md
# # final stage/image
# FROM mcr.microsoft.com/dotnet/runtime-deps:7.0-alpine
# WORKDIR /app
# COPY --from=build /app/out .
# ENTRYPOINT ["dotnet", "dotnet.dll"]

FROM ubuntu 

RUN apt-get update 
RUN apt-get install -y nginx 
CMD [“echo”,”Image created”] 
