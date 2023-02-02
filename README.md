# vesta-php-fpm-80
VestaCP PHP templates for PHP 8.0

Usage:

```
apt-get install php8.0-apcu php8.0-mbstring php8.0-bcmath php8.0-cli php8.0-curl php8.0-fpm php8.0-gd php8.0-intl php8.0-mysql php8.0-soap php8.0-xml php8.0-zip php8.0-memcache php8.0-memcached php8.0-zip
update-rc.d php8.0-fpm defaults
a2enconf php8.0-fpm
systemctl restart apache2
cp -r /etc/php/8.0/ /root/vst_install_backups/php8.0/
rm -f /etc/php/8.0/fpm/pool.d/*
wget https://github.com/t0rik/vesta-php-fpm-80/raw/master/PHP-FPM-80.stpl -O /usr/local/vesta/data/templates/web/apache2/PHP-FPM-80.stpl
wget https://raw.githubusercontent.com/t0rik/vesta-php-fpm-80/main/PHP-FPM-80.tpl -O /usr/local/vesta/data/templates/web/apache2/PHP-FPM-80.tpl
wget https://raw.githubusercontent.com/t0rik/vesta-php-fpm-80/master/PHP-FPM-80.sh -O /usr/local/vesta/data/templates/web/apache2/PHP-FPM-80.sh
chmod a+x /usr/local/vesta/data/templates/web/apache2/PHP-FPM-80.sh
```
