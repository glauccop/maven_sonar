     pipeline {
        agent none
        stages {
         
          stage("build & sonarqube") {
            agent any
            steps {
              withSonarQubeEnv('SonarQube') {
               cmd "mvn clean package sonar:sonar"
              }
            }
          }
        }
      }
