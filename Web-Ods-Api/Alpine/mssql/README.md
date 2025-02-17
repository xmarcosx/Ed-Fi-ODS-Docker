# Ed-Fi Web ODS/API
Provides docker deployment for Ed-Fi ODS/API [v5.1.0](https://techdocs.ed-fi.org/pages/viewpage.action?pageId=83788284) running SQL Server.

**NOTE: This image is suitable for production use.**

## Image Links
[2.0.0](https://github.com/Ed-Fi-Alliance-OSS/Ed-Fi-ODS-Docker/blob/v2.0.0/Web-Ods-Api/Alpine/mssql/Dockerfile)

## Image Variants
The only supported image at this time is an Alpine-based implementation.

`edfialliance/ods-api-web-api:<version>`

## Supported Environment Variables
```
API_MODE=<Value that will replace ApiSettings.Mode in app.settings.json, i.e. YearSpecific>
LOGS_FOLDER=<path to store the log files>
ODS_VIRTUAL_NAME=<virtual name for the ods endpoint>
SQLSERVER_ODS_DATASOURCE=<DNS or IP Address of the SQL Server Instance, i.e. sql.somedns.org or 10.1.5.9,1433
SQLSERVER_ADMIN_DATASOURCE=<DNS or IP Address of the SQL Server Instance that contains the Admin/Security/Master databases, i.e. sql.somedns.org or 10.1.5.9,1433>
SQLSERVER_USER=<SQL Username with access to SQL Server Ed-Fi databases, edfiadmin>
SQLSERVER_PASSWORD=<SQL Password for the SQLSERVER_USER with access to SQL Server Ed-Fi databases, password123!>
```

## License Information
View [license information](https://github.com/Ed-Fi-Alliance-OSS/Ed-Fi-ODS-Docker/blob/main/LICENSE) for the software contained in this image.

As with all Docker images, these likely also contain other software which may be under other licenses (such as Bash, etc. from the base distribution, along with any direct or indirect dependencies of the primary software being contained).

As for any pre-built image usage, it is the image user's responsibility to ensure that any use of this image complies with any relevant licenses for all software contained within.
