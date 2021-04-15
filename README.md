# MAD-DB-CleanBackup
periodic Cleanup and Backup Docker for MAD DB

Fill in docker-compose.yml the MariaDB Container Name / MariaDB DB Name / MariaDB Root Password and

"docker-compose up -d periodic-cleanup"

It will backup and pack (GZIP) the complete DB in /periodic-cleanup/mysql/backup Folder and then clean DB table pokemon -> entrys older than 7 days, every day.
Timediff for cleanup can be customized in \periodic-cleanup\scripts\daily\cleanup-database file.
