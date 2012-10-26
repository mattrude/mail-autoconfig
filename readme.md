# Mail Client Auto Configuration Site

This is the autoconfig file for [Thunderbird](http://www.mozilla.org/en-US/thunderbird/) and other mail clients.

It is expected to be accessible via autoconfig.example.com. 

## Web Server Configurations

Below are example web server config for this site.

### Nginx Server

    server {
        listen 80;
        listen [::]:80;
        server_name autoconfig.example.com autoconfig.example.org autoconfig.example.net;
        root /var/www/mail-autoconfig;
    }

### Apache Server

    <VirtualHost *:80>
        ServerName autoconfig.example.com
        DocumentRoot /var/www/mail-autoconfig
    </VirtualHost>

## Other Resources

* https://developer.mozilla.org/en/Thunderbird/Autoconfiguration/FileFormat/HowTo
* https://developer.mozilla.org/en-US/docs/Thunderbird/Autoconfiguration
