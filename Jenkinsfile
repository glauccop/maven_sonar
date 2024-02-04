     pipeline {
        agent none
        stages {
         
          stage("build & sonarqube") {
            agent any
            steps {
              withSonarQubeEnv('SonarQube_TOKEN') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
