# Nextcloud

## First Run Setup

### Add Configuration For NGINX

nginx.conf and mime.types to be put in the Configuration/NGINX directory.

Included nginx.conf has only a few minor tweaks from the one located here:

https://docs.nextcloud.com/server/stable/admin_manual/installation/nginx.html#nextcloud-in-the-webroot-of-nginx

??? Template 1.conf is WITHOUT Collabora

??? Template 2.conf is WITH Collabora

### Add Your Domain as a Trusted Domain

[Official Documentation](https://docs.nextcloud.com/server/latest/admin_manual/installation/installation_wizard.html#trusted-domains)

* Open the "config.php" file, located in `<Stack Directory>/Application/config`.
* Under the "trusted_domains" array, add `1 => 'cloud.williammiceli.systems',`.

### Apache Configuration Reference

https://docs.nextcloud.com/server/stable/admin_manual/installation/source_installation.html?

### Setup trusted domains on first startup

https://docs.nextcloud.com/server/14/admin_manual/installation/installation_wizard.html#trusted-domains

## Useful Tools

* [Official Security Check](https://scan.nextcloud.com/)

## To-Do's

* Explain how to manually setup Redis