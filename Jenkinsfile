     pipeline {
        agent none
        stages {
         
          stage("build & sonarqube") {
            agent any
            steps {
              withSonarQubeEnv('SonarQube') {
                mvn clean package sonar:sonar
              }
            }
          }
        }
      }
