# WilliamMiceli's Personal Rancher Catalog

My personal rancher catalog to make my own life just a little bit easier.
Hopefully it can also be of use to others as well!

## TODO List

* Have DATA_DIR be optional
* Include logos for all stacks
* Include descriptions and setup instructions for all stacks

## Stack Completion Statuses

- [ ] Adminer - [Docker Hub](https://hub.docker.com/_/adminer) - [Website](https://www.adminer.org/en/)
- [x] Apache Guacamole - [Docker Hub](https://hub.docker.com/r/guacamole/guacamole) - [Website](https://guacamole.apache.org/)
- [x] Bind - [Docker Hub](https://hub.docker.com/r/sameersbn/bind)
- [ ] Discourse - [Docker Hub](https://hub.docker.com/_/discourse) - [Website](https://www.discourse.org/)
- [ ] Drupal - [Docker Hub](https://hub.docker.com/_/drupal) - [Website](https://www.drupal.org/)
- [ ] Eclipse Che - [Docker Hub](https://hub.docker.com/_/eclipse-che) - [Website](https://www.eclipse.org/che/)
- [x] Ghost - [Docker Hub](https://hub.docker.com/_/ghost) - [Website](https://ghost.org/)
- [ ] Gitea - [Docker Hub](https://hub.docker.com/r/gitea/gitea) - [Website](https://gitea.io/en-us/)
- [ ] GitPitch Pro - [Docker Hub](https://hub.docker.com/_/gitpitch-pro) - [Website](https://gitpitch.com/)
- [ ] Gogs - [Docker Hub](https://hub.docker.com/r/gogs/gogs) - [Website](https://gogs.io/)
- [ ] Grafana - [Docker Hub](https://hub.docker.com/r/grafana/grafana) - [Website](https://grafana.com/)
- [x] HTTPD - [Docker Hub](https://hub.docker.com/_/httpd) - [Website](http://httpd.apache.org/)
- [x] InvoiceNinja - [Docker Hub](https://hub.docker.com/r/invoiceninja/invoiceninja) - [Website](https://www.invoiceninja.org/)
- [ ] Joomla - [Docker Hub](https://hub.docker.com/_/joomla) - [Website](https://www.joomla.org/)
- [ ] Logstash - [Docker Hub](https://hub.docker.com/_/logstash) - [Website](https://www.elastic.co/products/logstash)
- [ ] Matomo - [Docker Hub](https://hub.docker.com/_/matomo) - [Website](https://matomo.org/)
- [ ] MediaWiki - [Docker Hub](https://hub.docker.com/_/mediawiki) - [Website](https://www.mediawiki.org/)
- [ ] Memcached - [Docker Hub](https://hub.docker.com/_/memcached) - [Website](https://www.memcached.org/)
- [ ] MySQL - [Docker Hub](https://hub.docker.com/_/mysql) - [Website](https://www.mysql.com/)
- [x] Nextcloud - [Docker Hub](https://hub.docker.com/_/nextcloud) - [Website](https://nextcloud.com/)
- [ ] Nginx - [Docker Hub](https://hub.docker.com/_/nginx) - [Website](https://www.nginx.com/)
- [x] OpenProject - [Docker Hub](https://hub.docker.com/r/openproject/community) - [Website](https://www.openproject.org/)
- [x] PHPMyAdmin - [Docker Hub](https://hub.docker.com/r/phpmyadmin/phpmyadmin) - [Website](https://www.phpmyadmin.net/)
- [ ] PostgreSQL - [Docker Hub](https://hub.docker.com/_/postgres) - [Website](https://www.postgresql.org/)
- [ ] ProjectSend - [Docker Hub](https://hub.docker.com/r/linuxserver/projectsend) - [Website](https://www.projectsend.org/)
- [ ] Pydio Cells - [Docker Hub](https://hub.docker.com/r/pydio/cells/) - [Website](https://pydio.com/en/)
- [ ] Redis - [Docker Hub](https://hub.docker.com/_/redis) - [Website](https://redis.io/)
- [ ] Redmine - [Docker Hub](https://hub.docker.com/_/redmine) - [Website](http://www.redmine.org/)
- [ ] Rocket.Chat - [Docker Hub](https://hub.docker.com/_/rocketchat) - [Website](https://rocket.chat/)
- [x] Snipe-IT - [Docker Hub](https://hub.docker.com/r/snipe/snipe-it) - [Website](https://snipeitapp.com/)
- [x] Traefik - [Docker Hub](https://hub.docker.com/_/traefik) - [Website](https://traefik.io/)
- [ ] Transmission - [Docker Hub](https://hub.docker.com/r/linuxserver/transmission) - [Website](https://transmissionbt.com/)
- [x] WordPress - [Docker Hub](https://hub.docker.com/_/wordpress) - [Website](https://wordpress.com/)
- [x] XWiki - [Docker Hub](https://hub.docker.com/_/xwiki) - [Website](https://www.xwiki.org/)
- [ ] YOURLS - [Docker Hub](https://hub.docker.com/_/yourls) - [Website](http://yourls.org/)

## Using These Templates For Non-Rancher Configurations

* Rancher provides networking for stacks, so any declarations to `networks` and `expose` are ignored (excluding `ports`) on creation.
  * Instead, network policies can be created within Rancher's "Environments"