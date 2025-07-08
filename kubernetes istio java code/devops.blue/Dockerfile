# Build command
#
# 1. [Linux/Mac] : ./gradlew clean bootJar 
#    [Windows]   : .\gradlew clean bootJar
# 2. docker build --tag devops-blue:1.0.0 . 
# 3. docker login (optional)
# 4. docker tag devops-blue:1.0.0 gaurav0081/devops-blue:1.0.0
# 5. docker push gaurav0081/devops-blue:1.0.0

# .\gradlew clean bootJar && docker build --tag devops-blue:1.0.0 . && docker tag devops-blue:1.0.0 gaurav0081/devops-blue:1.0.0 && docker push timpamungkas/devops-blue:1.0.0

FROM amazoncorretto:17

ARG JAR_FILE=build/libs/devops-blue.jar

ADD ${JAR_FILE} devops-blue.jar

ENTRYPOINT ["java", "-jar", "devops-blue.jar"]