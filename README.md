Installing Apache and Updating the Firewall

    sudo apt update
    sudo apt upgrade
    sudo apt install apache2

    sudo ufw app list

    sudo ufw app info "Apache Full"

    sudo ufw allow in "Apache Full"

APACHE INSTALLED SUCCESFULLY TILL HERE, YOU CAN CHECK BY ENTERING YOUR PUBLIC IP OR PUBLICK DNS ADDRESS - http://your_server_ip

==================================================

    sudo systemctl restart apache2
    sudo systemctl status apache2

    ============================

Basic permissions below:

User Permission : sudo chown -R ubuntu:root /var/www/html

sudo find html -type d -exec chmod 775 {} \;
sudo find html -type f -exec chmod 664 {} \;

===============================

FOR ZIP AND UNZIP MODULE - USEFUL

sudo apt-get install zip unzip
