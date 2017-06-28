# Dropbox in Docker

[![Docker Pulls](https://img.shields.io/docker/pulls/janeczku/dropbox.svg?maxAge=2592000)][hub]
[![License](https://img.shields.io/github/license/janeczku/docker-alpine-kubernetes.svg?maxAge=2592000)]()

[hub]: https://hub.docker.com/r/janeczku/dropbox/

Run Dropbox inside Docker. Fully working with local host folder mount or inter-container linking (via `--volumes-from`).
This version also allows tray bar indicator to be shown.
There is also a shell script as a shortcut for most common used commands.


## Usage examples

### Quickstart

    ./dropbox-docker install (path_to_dropbox_folder)
    ./dropbox-docker start


Check the logs of the container to get URL to authenticate with your Dropbox account.

    ./dropbox-docker log

Copy and paste the URL in a browser and login to your Dropbox account to associate.

You should see something like this:

> "This computer is now linked to Dropbox. Welcome xxxx"

## Manage exclusions and check sync status

    ./dropbox-docker help

Any other command can be sent by replacing "dropbox" with "dropbox-docker".
There is also a possibility to start shell session inside the container

    ./dropbox-docker bash

## ENV variables & Exposed volumes
Modify "dropbox-docker" shell script

