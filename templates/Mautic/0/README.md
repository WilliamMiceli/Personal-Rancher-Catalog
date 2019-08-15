# Nextcloud

Nextcloud offers industry-leading on-premises file sync and online collaboration technology. Our expertise is in combining the convenience and ease of use of consumer-grade solutions like Dropbox and Google Drive with the security, privacy and control business needs.

Our self-hosted solutions ensure you know where data is, who has access, and that even meta-data does not leak.

## Pre-Requisites

* Traefik deployed

## Useful Tools

* [Official Security Check](https://scan.nextcloud.com/)

## Easy Redis Setup

Copy the "redis.config.php" file into your Configuration directory.
You may need to restart your stack for it to pick up.
You can monitor if it is working by opening a shell terminal on your Redis container and using `redis-cli MONITOR`

## To-Do's

* Explain how to manually setup Redis
* Fix Cron container, does not yet properly execute yet
* Better setup trusted_proxies
  * [Documentation Reference](https://docs.nextcloud.com/server/stable/admin_manual/configuration_server/reverse_proxy_configuration.html?highlight=reverse%20proxy)
* Create my own Nextcloud image and make the following changes:
  * Add the Redis config
  * Add the reverse proxy config
  * Have the entrypoint automatically run the "php occ db:add-missing-indices"