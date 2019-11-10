# WilliamMiceli's Personal Rancher Catalog

My personal rancher catalog to make my own life just a little bit easier.
Hopefully it can also be of use to others as well!

## TODO List

- Finish what I've started
- Have DATA_DIR be optional
- Include logos for all stacks
- Include descriptions and setup instructions for all stacks

## Stack Completion Overview

- [ ] Adminer ([Docker Hub](https://hub.docker.com/_/adminer) | [Website](https://www.adminer.org/en/))
- [x] Bind ([Docker Hub](https://hub.docker.com/r/sameersbn/bind))
- [ ] Discourse ([Docker Hub](https://hub.docker.com/_/discourse) | [Website](https://www.discourse.org/))
- [ ] Drupal ([Docker Hub](https://hub.docker.com/_/drupal) | [Website](https://www.drupal.org/))
- [x] Ghost ([Docker Hub](https://hub.docker.com/_/ghost) | [Website](https://ghost.org/))
- [x] Gitea ([Docker Hub](https://hub.docker.com/r/gitea/gitea) | [Website](https://gitea.io/en-us/))
- [x] GitLab ([Docker Hub](https://hub.docker.com/r/gitlab/gitlab-ce) | [Website](https://about.gitlab.com/))
- [x] GitLab Runner ([Docker Hub](https://hub.docker.com/r/gitlab/gitlab-runner) | [Website](https://docs.gitlab.com/runner/))
- [ ] GitPitch Pro ([Docker Hub](https://hub.docker.com/_/gitpitch-pro) | [Website](https://gitpitch.com/))
- [ ] Grafana ([Docker Hub](https://hub.docker.com/r/grafana/grafana) | [Website](https://grafana.com/))
- [x] Grav ([Docker Hub](https://hub.docker.com/r/williammiceli/grav) | [Website](https://getgrav.org/))
- [x] HTTPD ([Docker Hub](https://hub.docker.com/_/httpd) | [Website](http://httpd.apache.org/))
- [x] InvoiceNinja ([Docker Hub](https://hub.docker.com/r/invoiceninja/invoiceninja) | [Website](https://www.invoiceninja.org/))
- [x] Jellyfin ([Docker Hub](https://hub.docker.com/r/jellyfin/jellyfin) | [Website](https://jellyfin.github.io/))
- [ ] Joomla ([Docker Hub](https://hub.docker.com/_/joomla) | [Website](https://www.joomla.org/))
- [ ] Matomo ([Docker Hub](https://hub.docker.com/_/matomo) | [Website](https://matomo.org/))
- [ ] Memcached ([Docker Hub](https://hub.docker.com/_/memcached) | [Website](https://www.memcached.org/))
- [ ] MongoDB ([Docker Hub](https://hub.docker.com/_/mongo) | [Website](https://www.mongodb.com/))
- [ ] MySQL ([Docker Hub](https://hub.docker.com/_/mysql) | [Website](https://www.mysql.com/))
- [x] Nextcloud ([Docker Hub](https://hub.docker.com/_/nextcloud) | [Website](https://nextcloud.com/))
- [x] Nginx ([Docker Hub](https://hub.docker.com/_/nginx) | [Website](https://www.nginx.com/))
- [ ] Node RED ([Docker Hub](https://hub.docker.com/r/nodered/node-red-docker) | [Website](https://nodered.org/))
- [x] OpenProject ([Docker Hub](https://hub.docker.com/r/openproject/community) | [Website](https://www.openproject.org/))
- [x] PHPMyAdmin ([Docker Hub](https://hub.docker.com/r/phpmyadmin/phpmyadmin) | [Website](https://www.phpmyadmin.net/))
- [ ] PostgreSQL ([Docker Hub](https://hub.docker.com/_/postgres) | [Website](https://www.postgresql.org/))
- [ ] Redis ([Docker Hub](https://hub.docker.com/_/redis) | [Website](https://redis.io/))
- [ ] Redmine ([Docker Hub](https://hub.docker.com/_/redmine) | [Website](http://www.redmine.org/))
- [ ] Rocket.Chat ([Docker Hub](https://hub.docker.com/r/rocketchat/rocket.chat) | [Website](https://rocket.chat/))
- [x] Snipe-IT ([Docker Hub](https://hub.docker.com/r/snipe/snipe-it) | [Website](https://snipeitapp.com/))
- [ ] sysPass ([Docker Hub](https://hub.docker.com/r/syspass/syspass) | [Website](https://www.syspass.org/en))
- [x] Traefik ([Docker Hub](https://hub.docker.com/_/traefik) | [Website](https://traefik.io/))
- [x] Wiki.js v1 ([Docker Hub](https://hub.docker.com/r/requarks/wiki/) | [Website](https://wiki.js.org/))
- [x] WordPress ([Docker Hub](https://hub.docker.com/_/wordpress) | [Website](https://wordpress.com/))

### Will Complete at a Later Date

- Transmission ([Docker Hub](https://hub.docker.com/r/linuxserver/transmission) | [Website](https://transmissionbt.com/))

### Archived (May Or May Not Be Completed)

- Guacamole ([Docker Hub](https://hub.docker.com/r/guacamole/guacamole) | [Website](https://guacamole.apache.org/))
- Logstash ([Docker Hub](https://hub.docker.com/_/logstash) | [Website](https://www.elastic.co/products/logstash))
- Mautic ([Docker Hub](https://hub.docker.com/r/mautic/mautic) | [Website](https://www.mautic.org/))
- MediaWiki ([Docker Hub](https://hub.docker.com/_/mediawiki) | [Website](https://www.mediawiki.org/))
- Pydio Cells ([Docker Hub](https://hub.docker.com/r/pydio/cells/) | [Website](https://pydio.com/en/))
- XWiki ([Docker Hub](https://hub.docker.com/_/xwiki) | [Website](https://www.xwiki.org/))
- YOURLS ([Docker Hub](https://hub.docker.com/_/yourls) | [Website](http://yourls.org/))

### Removed/Ignored

- Gogs ([Docker Hub](https://hub.docker.com/r/gogs/gogs) | [Website](https://gogs.io/)) - Gitea has far surpassed Gogs in many ways, to the point where I can't find a reason to use Gogs over Gitea, so I don't believe there would be any reason to keep a configuration around for it.
- Eclipse Che ([Docker Hub](https://hub.docker.com/_/eclipse-che) | [Website](https://www.eclipse.org/che/)) - It currently looks like Che 7 will require kubernetes and other requirements to have setup, and running it on Docker is even more complicated. Not worth it to me to try putting it together here.

## Using These Templates For Non-Rancher Configurations

- Rancher provides networking for stacks, so any declarations to `networks` and `expose` are ignored (excluding `ports`).
  - Instead, network policies can be created within Rancher's "Environments"
