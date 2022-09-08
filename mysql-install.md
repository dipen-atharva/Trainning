
# How To Install MySQL on Linux




Update the system packages to the latest versions:

> `sudo apt update && sudo apt upgrade`

##### Installing MySql

Run the following command to install MySql;

> `sudo apt install mysql-server`

<!-- ##### Now confirm the installation -->

Now confirm the installation and check MySQL version typing following command:

> `mysql -V`

After completing installation MySQL will start automatically. Check MySQL version by typing:

> `sudo systemctl status mysql`

The output something like below:

```
mysql.service - MySQL Community Server
   Loaded: loaded (/lib/systemd/system/mysql.service; enabled; vendor preset: enabled)
   Active: active (running) since Wed 2018-06-20 11:30:23 PDT; 5min ago
 Main PID: 17382 (mysqld)
    Tasks: 27 (limit: 2321)
   CGroup: /system.slice/mysql.service
           -17382 /usr/sbin/mysqld --daemonize --pid-file=/run/mysqld/mysqld.pid
```

##### Start MySql Console by typing

> `mysql -u root -p`

##### Setting Up MySQL

> `sudo mysql_secure_installation`

The above command will take you to different prompts. In the first prompt, it will ask you to configure Validate Password Plugin which is used to set password validation strength and the levels are low, medium and high. You can prefer any of the strength levels you want to set. If you don’t want to set up the Validate Password Plugin just press ENTER. In the next prompts, you will be asked questions about increasing Security of MySQL. It is recommended to answer ‘Y’ for all questions asked during secure installation.

### Detailed Guide
* [How to install Mysql Server](https://phoenixnap.com/kb/install-mysql-ubuntu-20-04)
