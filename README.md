# DockerMysqlAzureBackup
Docker container for automated daily backups of a MySQL database to Azure Storage. Get on [Docker hub](https://hub.docker.com/r/smeykk/mysql-azure-backup).

### Environment variables:
- `MYSQL_CONTAINER_NAME` - The MySQL host
- `MYSQL_DATABASE` - Database name
- `MYSQL_USER` - MySQL user with backup permissions
- `MYSQL_PASSWORD` - MySQL user password
- `BLOB_NAME` - Name of the Azure Storage Blob (`{BLOB_NAME}-yyyy-MM-dd_HH:mm` format)
- `CONTAINER` - Azure Storage container name
- `AZURE_STORAGE_ACCOUNT` - Azure Storage account name
- `AZURE_STORAGE_ACCESS_KEY` - Azure Storage account access key