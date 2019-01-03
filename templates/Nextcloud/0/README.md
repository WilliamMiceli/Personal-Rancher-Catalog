# Nextcloud

## First Run Setup

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