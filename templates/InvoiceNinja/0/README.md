# Invoice Ninja

[Hosted Official Website](https://www.invoiceninja.com/)

[Self-Hosted Official Website](https://www.invoiceninja.org/)

[Docker Page](https://hub.docker.com/r/invoiceninja/invoiceninja/)

## Description

  Free Open-Source Invoicing

  Expenses & time-tracking built with Laravel

## Pre-Deployment

### Optional Features Preparation

#### Google Maps Integration

1. [Get an API Key Here](https://developers.google.com/maps/documentation/javascript/get-api-key).
2. Insert `GOOGLE_MAPS_API_KEY=<Your API Key>` into your .env file.

### Required Configuration Files

* Place a "nginx.conf" file in the `<Stack Directory>/Configuration` directory.
  * An Example can be found in the "Resources" directory for this catalog item.
    * This file has been modified for this configuration, based on the [Example](https://github.com/invoiceninja/dockerfiles/blob/master/docker-compose/nginx.conf) located in the official GitHub repository.
* Place a ".env" file in the `<Stack Directory>/Configuration` directory.
  * An example can be found in the "Resources" directory for this catalog item.
    * This file has been modified for this configuration, based on the ".env.example" file provided within the container image.
  * [A Configuration Guide](https://invoice-ninja.readthedocs.io/en/latest/configure.html) related to environment variables, along with the [Full Example](https://github.com/invoiceninja/invoiceninja/blob/master/.env.example) from the official GitHub repository.

## Tips

* With this configuration, DO NOT enable "Require HTTPS", as the connection between Traefik and InvoiceNinja is over non-SSL HTTP, and is not setup for internal HTTPS.

## Backing Up Your Instance

### Complete Backup

Through the MySQL container, run a MySQL Dump.
(Will complete this later)

### Easy Backup

The web interface provides an easy backup method by exporting to a JSON file, which saves most information.

## TODO

* Add more integration instructions
* Add better trusted proxies configuration