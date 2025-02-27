---
title: "Configuration"
weight: 14
---
## Getting started

This project requires Go to be installed. On OS X with Homebrew you can just run `brew install go`.





make a copy of [conf/importer-example.yml](https://github.com/netsage-project/grafana-dashboard-manager/blob/master/conf/importer-example.yml) and name it `conf/importer.yml` You'll need GRAFANA ADMINISTRATIVE privileges to proceed.


### Authentication


You can use either an Auth Token or username/password credentials.  If you configure both then the Token is given priority.

Watched folders under grafana is a white list of folders that are being managed by the tool.  By default only "General" is managed.  

env.output defines where the files will be saved and imported from.

### Global Flags

`globals.debug` when set will print a more verbose output (Development In Progress)
`globals.ignore_ssl_errors` when set will disregard any SSL errors and proceed as expected


### Building/Running the app

Running it then should be as simple as:

```bash
$ make build
$ ./bin/grafana-dashboard-manager
```
