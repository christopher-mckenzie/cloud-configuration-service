## config service 

* used to implement spring config server
* intermediary between spring applications and a version-controlled repository of config files
* to standup a config server add @EnableConfigServer over Application main
* use spring.cloud.config.server.git.uri in yml file to define url for config files
* to change value returned from config server
    * in config files update value
    * to verify changes http://localhost:<config-server-port>/<application-name>/<active-profile>
    * to have application reflect changes go to http://localhost:<client-port>/actuator/refresh (must be a post and can be empty)
    * to see changes go to clients message endpoint
    
## tutorial

* documentation: https://spring.io/guides/gs/centralized-configuration/