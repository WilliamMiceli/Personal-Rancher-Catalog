# Eclipse Che (Single User)

[Official Website](https://www.eclipse.org/che/)
[Docker Page](https://hub.docker.com/r/eclipse/che/)

[v6 Documentation](https://www.eclipse.org/che/docs/6/che/docs/index.html)









##### CLI Reference

USAGE:
`  docker run -it --rm *<DOCKER_PARAMETERS>* eclipse/che-cli:*<version>* *[COMMAND]*`

MANDATORY DOCKER PARAMETERS:
```  -v *<LOCAL_PATH>*:/data```            Where user, instance, and log data saved

OPTIONAL DOCKER PARAMETERS:
`  -e CHE_HOST=*<YOUR_HOST>*`              IP address or hostname where che will serve its users
`  -e CHE_PORT=*<YOUR_PORT>*`              Port where che will bind itself to
`  -e CHE_CONTAINER=*<YOUR_NAME>*`         Prefix name for the che container
`  -v *<LOCAL_PATH>*:/data/instance`       Where instance, user, log data will be saved
`  -v *<LOCAL_PATH>*:/data/backup`         Where backup files will be saved
`  -v *<LOCAL_PATH>*:/repo`                che git repo - uses local binaries and manifests
`  -v *<LOCAL_PATH>*:/assembly`            che assembly - uses local binaries
`  -v *<LOCAL_PATH>*:/sync`                Where remote ws files will be copied with sync command
`  -v *<LOCAL_PATH>*:/unison`              Where unison profile for optimizing sync command resides
`  -v *<LOCAL_PATH>*:/chedir`              Soure repository to convert into workspace with Chedir utility

COMMANDS:
`  action *<action-name>*`                 Start action on che instance
`  backup`                                 Backups che configuration and data to /data/backup volume mount
`  config`                                 Generates a che config from vars; run on any start / restart
`  destroy`                                Stops services, and deletes che instance data
`  dir *<command>*`                        Use Chedir and Chefile in the directory mounted to :/chedir
`  download`                               Pulls Docker images for the current che version
`  help`                                   This message
`  info`                                   Displays info about che and the CLI
`  init`                                   Initializes a directory with a che install
`  offline`                                Saves che Docker images into TAR files for offline install
`  restart`                                Restart che services
`  restore`                                Restores che configuration and data from /data/backup mount
`  rmi`                                    Removes the Docker images for <version>, forcing a repull
`  ssh *<wksp-name>* *[machine-name]*`     SSH to a workspace if SSH agent enabled
`  start`                                  Starts che services
`  stop`                                   Stops che services
`  sync *<wksp-name>*`                     Synchronize workspace with local directory mounted to :/sync
`  test *<test-name>*`                     Start test on che instance
`  upgrade`                                Upgrades che from one version to another with migrations and backups
`  version`                                Installed version and upgrade paths

GLOBAL COMMAND OPTIONS:
`  --fast`                                 Skips networking, version, nightly and preflight checks
`  --offline`                              Runs CLI in offline mode, loading images from disk
`  --debug`                                Enable debugging of che server
`  --trace`                                Activates trace output for debugging CLI