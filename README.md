# mypics

- Prerequisites
1. OS ubuntu14.04 or next version
2. PHP 7.0.22-2+ or next version
3. MySql 5.6 or next version

1. Clone repository
git clone git@github.com:priyanka-mohite/mypics.git

2. Create virtul host
<VirtualHost *:80>
        <Directory /var/www/>
                Options Indexes FollowSymLinks
                AllowOverride All
                Require all granted
        </Directory>

        ServerAdmin admin@example.com
        ServerName my-magento.local.com
        ServerAlias my-magento.local.com
        DocumentRoot /var/www/magento
        ErrorLog ${APACHE_LOG_DIR}/error.log
        CustomLog ${APACHE_LOG_DIR}/access.log combined
</VirtualHost>

3. Open URL into browser
- First it will check for all local dependencies for magento 2.
- Install all dependencies.
- Add application URL my-magento.local.com
- Add admin URL my-magento.local.com/admin
- Add database description {username,password,databasename:"magento",database prefix:"mag_"}

4. If done successfully you will land to home page and can login in admin section.