## config service 

* used to implement spring config server
* intermediary between spring applications and a version-controlled repository of config files
* to standup a config server add @EnableConfigServer over Application main
* use spring.cloud.config.server.git.uri in yml file to define url for config files