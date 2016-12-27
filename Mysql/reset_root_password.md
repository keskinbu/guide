## Reset Root Password
```
mysql -u root
USE mysql;
UPDATE user SET password=PASSWORD("NEWPASSWORD") WHERE User='root';
FLUSH PRIVILEGES;
quit
```

## Export and Import sql file using command line

```
mysqldump -u root -p --opt --all-databases > alldb.sql
mysql -u root -p < alldb.sql
```
