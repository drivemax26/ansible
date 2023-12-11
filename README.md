This repository contains an application developed on the [Laravel](https://laravel.com/) framework - https://github.com/Practical-DevOps/app-for-devops.

The task is to write the `main.yml` Ansible playbook for automating the installation and configuration of an Apache server with this application and a MariaDB server on two machines running Ubuntu 22.04. The playbook should adhere to the following requirements:

The web server is included in the group named `[server]`, and the database server is included in the group `[db]`.
Variables named `db_host`, `db_name`, `db_user`, `db_pass` are defined to configure the connection between the application and the database.
Here is an example of launching the playbook to install the application on an Apache web server with a MariaDB database server:

```bash
ansible-playbook main.yml --extra-vars "db_host=db.some.net db_name=app_db db_user=app_user db_pass=app_pass"
```
