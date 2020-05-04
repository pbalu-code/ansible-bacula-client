# ansible-bacula-client
Centos/RedHat (7, 8), Ubuntu 18 Bacula client install with Mysql/MariaDB and PostgreSQL dump scripts.

#Usage

Declare variables as you need:
```yaml
bacula_server: (default: 'bacula')
bacula_client_pw: (default: 'bacula')
bacula_exclude_sql_db: (defaults:)
  - information_schema
  - mysql
  - performance_schema
  - demo
  - template
  - postgres
bacula_scripts: (default: /usr/local/sbin/bacula)
bacula_sql_dumps_folder: (default: /var/bacula)
bacula_mysql_user: (default: 'root')
bacula_mysql_user_password: (default: '')
bacula_pgsql_user: (default: postgres)
keep_backups_days: (default: 5)
```