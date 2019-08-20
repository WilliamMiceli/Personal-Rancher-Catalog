# Guacamole

Apache Guacamole is a clientless remote desktop gateway. It supports standard protocols like VNC, RDP, and SSH.

We call it clientless because no plugins or client software are required.

Thanks to HTML5, once Guacamole is installed on a server, all you need to access your desktops is a web browser.

## Initial Setup

On the "guacamole" container, run:
`/opt/guacamole/bin/initdb.sh --mysql > /setup/initdb.sql`

On the "mysql" container, run:
`cat /setup/initdb.sql | mysql -u root -p guacamole_db`

## Post-Installation

Make sure you create your own user account and delete the "guacadmin" user (or at very least change the password)

## TODO
* Allow adding extensions