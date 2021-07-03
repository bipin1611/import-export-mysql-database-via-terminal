# Import and Export MySQL Database via Terminal Commands

Here you can find import and export database command which you use on hosted server. You can use while you don't have any import or export option on your server.

## #Import Database

Let's assume that you have install mysql on server in `/var/www/html/` directory

### Step 1:- Connect You Terminal via SSH

### Step 2:- Connect MySQL
use following command to connect

 ```
 mysql -u root -p
 ```
 
### Steep 3: Use Database or Create New
 
To Create New Datbase: `CREATE DATABASE dbname;`
 
 After that you need to use database which you want do to action on it, Run Following command
  ```
  use dbname
  ```
   
 ### Step 4: Import Database `.sql` File

 This  `dbname.sql` file shoud be exists in the current directory. Which is `/var/www/html/`.
  ```
  source dbname.sql
  ```
  This will import into database.


## #Export Database

### Step 1:- Connect You Terminal via SSH

### Step 2:- Run `mysqldump` Command

By running this command, it will export in the current directory.

 ```
 mysqldump -u root dbaname > "/var/www/html/filename.sql" 
 ```
 Please make sure that you should run command on directory which mysql installed on.
 
## Contact Me
Please let me know if you face any issue. Send me Mail at [parmarbipin96013@gmail.com](mailto:parmarbipin96013@gmail.com)
 
 
