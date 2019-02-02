# Nextcloud

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