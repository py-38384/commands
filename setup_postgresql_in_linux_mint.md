
Upadte APT Packages

    sudo apt update

Install postgresql

    sudo apt install postgresql postgresql-contrib

Confirm postgres in running

    sudo systemctl status postgresql

Start if not running

    sudo systemctl start postgresql

check if php has the postgresql extensions installed

    php -m | grep pgsql

If not then install the extension

    sudo apt install php-pgsql

Get inside postgresql shell
    
    sudo -u postgres psql

Create a new postgresql user

    CREATE ROLE root_user WITH LOGIN PASSWORD 'superstrongpassword';

Make it a superuser

    ALTER ROLE root_user WITH SUPERUSER CREATEDB CREATEROLE REPLICATION;

Exit the postgresql shell
    
    \q

Setup postgresql database form laravel app in .env file 

    DB_CONNECTION=pgsql
    DB_HOST=127.0.0.1
    DB_PORT=5432
    DB_DATABASE=my_app_database
    DB_USERNAME=root_user
    DB_PASSWORD=superstrongpassword

If you want a database management softwere you can you "DBeaver".
The best free database management softwere.
make sure to download the community version





