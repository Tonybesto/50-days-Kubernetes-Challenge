

## Image Build Info

| Item      | Description |   
| :---        |    :----:   |  
| Base  | maven:3.5-jdk-8-alpine  |  
| Work Directory  |  /code |     
| Build Instructions  |  mvn package -D skipTests |  
| Ports | N/A |  
| Runtime Image | openjdk:8-jre-alpine |  
| Launch Command | java -jar target/worker-jar-with-dependencies.jar |  
