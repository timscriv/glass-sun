FROM microsoft/aspnetcore-build:2.0
ARG source
RUN node -v
WORKDIR /app
EXPOSE 80
COPY ${source:-obj/Docker/publish} .
ENTRYPOINT ["dotnet", "CadmiumCrocodile.dll"]
