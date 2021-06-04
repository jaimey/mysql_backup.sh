
# mysql_backup.sh

Script for automating the daily mysql backups


## Installation 
Descargar y aplicar permiso de ejecución
```bash 
wget -O ~/mysql_backup.sh https://raw.githubusercontent.com/jaimey/mysql_backup.sh/master/mysql_backup.sh
```
```bash 
chmod +x ~/mysql_backup.sh
```
Crear carpeta
```bash 
mkdir ~/backup/db
```
Agregar al Crontab
```bash 
crontab -e
```
```bash 
0 7,13,19 * * *  /root/mysql_backup.sh >/dev/null 2>&1
```
    
