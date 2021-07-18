# CICD--Pipeline--for--user-management-service

## Steps to follow for CICD Pipeline on aws

### build your project using this command
```javascript
mvn clean package
```
### Add buildspec.yml to your project
```javascript
version: 0.2

phases:
  build:
    commands:
      - echo Entered the build phase...
      - mvn clean package
  post_build:
    commands:
      -echo Build compeleted successfully
artifacts:
  files:
    -target/user-management-service.jar
  discard-paths: yes
```
### Create a Project in AWS CodeBuild with your github repo

### Create AWS BeanStalk for deploy you application

### Create AWS CodePipeline with github repo and AWS Beanstalk

## Condlusion

now you are ready to your application
