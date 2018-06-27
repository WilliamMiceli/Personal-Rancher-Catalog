# Invoice Ninja

[Hosted Official Website](https://www.invoiceninja.com/)

[Self-Hosted Official Website](https://www.invoiceninja.org/)

[Docker Page](https://hub.docker.com/r/invoiceninja/invoiceninja/)

## From Website

Free Open-Source Invoicing
Expenses & time-tracking built with Laravel

### Pre-Installation:

Make sure that you have a "nginx.conf" file located inside of the "Config" folder for the webserver to function.
Copying the default one located [on their GitHub](https://github.com/invoiceninja/dockerfiles/blob/master/docker-compose/nginx.conf) should be sufficient.

You may need to run "php artisan cache:clear", and then "chmod -R 777 storage" in the "App" and "Cron" containers if you are getting file permission errors.

### Post-Installation:

Google Maps:
Get an API Key [Here](https://developers.google.com/maps/documentation/javascript/get-api-key) first.
Then add GOOGLE_MAPS_API_KEY=<your key> in your .env file.