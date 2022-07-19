## before start for Mac OS you have to install mysql-client
    brew install mysql-client
  
 ## then follow the instruction display on the terminal after the installation is completed

## How to export mysql database in digitalocean
    mysqldump -h your-db-host-here.db.ondigitalocean.com -P 25060 -u doadmin -p --ssl-ca=./certs/ca.crt --set-gtid-purged=OFF source-db > dump.sql
  
 ## How to import mysql database to digitalocean database
    mysql -u doadmin -p -h your-db-host-here.db.ondigitalocean.com -P 25060 --ssl-ca=./certs/ca.crt target-db < dump.sql
