# Workshop Demo App

This applicatoin is used by the example42 [Ruby for Puppet training](https://example42.com/training/).
Within this dummy application we demo an application which can not be configured by managing config files, but which must be configured using a command.

Deploy this application to /opt/app by running `git clone https://github.com/tuxmea/workshop-demo-app /opt/app`

You then have an executable which will allow you to read, set and change config settings.

Usage of the app:

## Usage
    /opt/app/bin/app.exe
    Usage: /opt/app/bin/app.exe ['list', 'set', 'rm', 'version']
    
## Read config
    /opt/app/bin/app.exe list
    ---
    key: value
    loglevel: debug
    user: martin
    cachepath: /etc/app/cache

## Change or add config
    /opt/app/bin/app.exe set
    Usage: /opt/app/bin/app.exe set <key> <value>

## Remove config
    /opt/app/bin/app.exe rm
    Usage: /opt/app/bin/app.exe rm <key>

## Print app version
    /opt/app/bin/app.exe version
    app version: 3.1.2-git-e4f10ac
