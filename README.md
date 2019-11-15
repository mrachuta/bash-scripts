## Project name

This is not a project - this is a library of bash scripts.
Each of scripts was written due to private needs/requirements.

## Table of contents

* [General info](#general-info)
* [gdirvemounter](#gdrivemounter)
* [vpsconfigurator](#vpsconfigurator)
* [pgconfigurator](#pgconfigurator)
* [watchdocker](#watchdocker)

## General info

Each of the scripts is used to realize another task.
Scripts was written due to personally requirements.
You can use it, modify and do everything that you want.

## gdrivemounter

Script was prepared to be used together with google-drive-ocalmfuse
package. Because gdo has no service-agent, script can be easily adapted
as base for service daemon. It can be also used as separate script, to
manually mount and umount multiple (or single) drives.

## vpsconfigurator

Script is used to automate initial configuration of VPS.
It creates the new user, set password and install necessary software.
Still in development to exclude as much as possible manually typing.

## pgconfigurator

Script used to configure contenerized postgresql database.
To use script, mount it under: */docker-entrypoint-initdb.d/pgconfigurator.sh* with read/write permissions.
It will be executed automatically, when container will be created.

## watchdocker

Script checking for available container-image updates.
If there is no updated image available, update via apt
on base system inside container is performed.
Can be adapted as service-daemon via cron.
