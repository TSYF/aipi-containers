#sudo docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=KoA5P8I5A1FpeV" \
#    -p 1433:1433 --name sql1 --hostname sql1 \
#    -d \
#    mcr.microsoft.com/mssql/server:2019-latest


# sudo docker run -e "ACCEPT_EULA=Y" -e "MSSQL_SA_PASSWORD=KoA5P8I5A1FpeV"    -p 1433:1433 --name sqlserver2019 --hostname sqlserver    -d    mcr.microsoft.com/mssql/server:2019-latest

# sudo docker exec -it sql2019 "bash"
# /opt/mssql-tools/bin/sqlcmd -S localhost -U SA


FROM mcr.microsoft.com/mssql/server:2019-latest

ENV ENTRY /script/entrypoint.sh

COPY ./docker/entrypoint.sh $ENTRY

ENTRYPOINT $ENTRY