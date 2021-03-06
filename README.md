# Sample Swagger Client generated from Swagger Service API file

### How to generate the client code 

1. Copy the API file generated by the Swagger Service (ie. ```swagger.yml```) and paste it to ```src/main/resources/```. Make sure that the configuration of ```swagger-codegen-maven-plugin``` in ```pom.xml``` is set to read from this file.  Client code will be generated based on this file.
2. ```cd``` to the root of the project.
3. Run ```mvn clean compile```. This will generate the Client code, however some dependencies will be missing.
4. To fix the missing dependencies problem, copy everything from ```<dependencies> ... </dependencies>``` in the generated ```pom.xml``` and paste it to the project's ```pom.xml``` as it's own ```<dependencies> ... </dependencies>```.
5. Rerun ```mvn clean compile```.

### Useful readings

[https://blog.philipphauer.de/enriching-restful-services-swagger/](https://blog.philipphauer.de/enriching-restful-services-swagger/)