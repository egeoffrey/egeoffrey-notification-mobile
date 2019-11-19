# egeoffrey-notification-betamax_sms

This is an eGeoffrey notification package.

## Description

send out sms notifications (betamax voip service).

## Install

To install this package, run the following command from within your eGeoffrey installation directory:
```
egeoffrey-cli install egeoffrey-notification-betamax_sms
```
After the installation, remember to run also `egeoffrey-cli start` to ensure the Docker image of the package is effectively downloaded and started.
To validate the installation, go and visit the *'eGeoffrey Admin'* / *'Packages'* page of your eGeoffrey instance. All the modules, default configuration files and out-of-the-box contents if any will be automatically deployed and made available.
## Content

The following modules are included in this package.

For each module, if requiring a configuration file to start, its settings will be listed under *'Module configuration'*. Additionally, if the module is a service, the configuration expected to be provided by each registered sensor associated to the service is listed under *'Service configuration'*.

To configure each module included in this package, once started, click on the *'Edit Configuration'* button on the *'eGeoffrey Admin'* / *'Modules'* page of your eGeoffrey instance.
- **notification/betamax_sms**: send out sms notifications (betamax voip service)
  - Module configuration:
    - *from**: the phone number to be used as the from of the message (e.g. 112341231232)
    - *hostname**: the Betamax hostname of your service (e.g. www.frevoipdeal.com)
    - *username**: the username of your betamax account (e.g. username)
    - *password**: the password of your betamax account (e.g. password)
    - *ssl**: use SSL
    - *to**: recipient phone number(s), comma separated (e.g. 112341231232)

## Contribute

If you are the author of this package, simply clone the repository, apply any change you would need and run the following command from within this package's directory to commit your changes and automatically push them to Github:
```
egeoffrey-cli commit "<comment>"
```
After taking this action, remember you still need to build (see below) the package (e.g. the Docker image) to make it available for installation.

If you are a user willing to contribute to somebody's else package, submit your PR (Pull Request); the author will take care of validating your contributation, merging the new content and building a new version.

## Build

Building is required only if you are the author of the package. To build a Docker image and automatically push it to [Docker Hub](https://hub.docker.com/r/egeoffrey/egeoffrey-notification-betamax_sms), run the following command from within this package's directory:
```
egeoffrey-cli build egeoffrey-notification-betamax_sms <amd64|arm>
```

## Uninstall

To uninstall this package, run the following command from within your eGeoffrey installation directory:
```
egeoffrey-cli uninstall egeoffrey-notification-betamax_sms
```
Remember to run also `egeoffrey-cli start` to ensure the changes are correctly applied.
## Tags

The following tags are associated to this package:
```
notification sms voip
```

## Version

The version of this egeoffrey-notification-betamax_sms is 1.0-11 on the master branch.
