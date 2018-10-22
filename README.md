# zabbix-windows-mysql
UserParameters for Template DB MySQL to use with Zabbix agent on a windows machine

# How to use it
1. Check correct path of mysql executable, could depend on installed version and personal choices of path during installation
2. Check correct path of .my.cnf, this file contains user & password for executing the queries defined in user parameters view ```sample.my.cnf``` for an example. Select a user that as enough permissions to run it. 
3. Include the user parameters definitions using ```Include=c:\zabbix\conf\userparameter_mysql.conf``` or copying the content of ```userparameter_mysql.conf``` inside the ```zabbix_agentd.win.conf``` file.
4. Restart the agent