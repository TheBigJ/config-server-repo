# config-server-repo

  This repo served as config serve for my micro services POC.
  It constains properties or configuration for the various services used in project.
  
  
  Spring Cloud Config Server exposes the following REST endpoints to get application specific configuration properties:
  
1. /{application}/{profile}[/{label}]
2. /{application}-{profile}.yml
3. /{label}/{application}-{profile}.yml
4. /{application}-{profile}.properties
5. /{label}/{application}-{profile}.properties


Here {application} refers to value of spring.config.name property, {profile} is an active profile and {label} is an optional git label (defaults to “master”).

Now if you access the URL http://localhost:8888/catalogservice/default then you will get the following response with catalogservice default configuration details:
