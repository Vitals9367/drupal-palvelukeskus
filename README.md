# Your Drupal 9 project

Description of your project.

## Environments

Env | Branch | Drush alias | URL
--- | ------ | ----------- | ---
development | main | - | https:///drupal-palvelukeskus.docker.so/

## Requirements

You need to have these applications installed to operate on all environments:

- [Docker](https://github.com/druidfi/guidelines/blob/master/docs/docker.md)
- [Stonehenge](https://github.com/druidfi/stonehenge)
- For the new person: Your SSH public key needs to be added to servers

## Create and start the environment

For the first time (new project):

``
$ make new
``

And following times to start the environment:

``
$ make up
``

Create site based on database export:
``
$ make fresh
``

DB syncing from server is disabled for now, uncomment line 45 at `tools/make/project/install.mk` to enable.

NOTE: Change these according of the state of your project.

## Login to Drupal container

This will log you inside the app container:

```
$ make shell
```
