Upadte APT Packages

    sudo apt update

Install Apache Server

    sudo apt install apache2

To check if Apache is running

    sudo systemctl status apache2

Install Mysql Server

    sudo apt install mysql-server

To check if MySQL is running

    sudo systemctl status mysql

Check which PHP versions are available (install the latest)

    apt list php*

Install PHP

    sudo apt install php8.4

Check PHP Version

    php -v

Install PHP Mysqli And Some Necessary Extension For PhpMyAdmin

    sudo apt install php8.4-mysql php8.4-mbstring php8.4-zip php8.4-xml php8.4-mysql php8.4-curl

Enable PHP Mysqli

    sudo phpenmod mysqli

Add Authentication To The PhpMyAdmin Config File For Enableing Auto Login

    /* Authentication type */
    $cfg['Servers'][$i]['auth_type'] = 'config';
    $cfg['Servers'][$i]['user'] = 'username';
    $cfg['Servers'][$i]['password'] = 'password';
