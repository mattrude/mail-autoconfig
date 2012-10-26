# Mail Client Auto Configuration Site

This is the autoconfig file for [Thunderbird](http://www.mozilla.org/en-US/thunderbird/) and other mail clients.

It is expected to be accessible via autoconfig.example.com. Below is a example Nginx config for this site.

    server {
        listen 80;
        listen [::]:80;
        server_name autoconfig.example.com autoconfig.example.org autoconfig.example.net;
        root /var/www/mail-autoconfig;
    }

## Other Resources

* https://developer.mozilla.org/en/Thunderbird/Autoconfiguration/FileFormat/HowTo
* https://developer.mozilla.org/en-US/docs/Thunderbird/Autoconfiguration
