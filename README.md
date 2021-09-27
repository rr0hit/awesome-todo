# This is a Sample Catalog.

A stack/Catalog is a technical blueprint of your software product. It defines the resources (viz. databases, applications, cloud resources) and the relationships between them. 

Each resource is defined in its own directory. 

## In this directory

There are a bunch of config files in this repo to define certain metadata about your catalog.

### Stack.json

* In this file you define Common environment variables and Secrets you need to launch any environment.

* Optionally, you can specify default values for these variables/secrets.

* Stack.json is also used to specify plugins like the logging plugin to augment the functionality in all your environment.

### features.json

This file is to enable/disable facets features.

### security.json

This file is to enable/ configure security related stuff for your environments. Example contains some configs related to Falco. 

### networking.json

Networking related configurations

