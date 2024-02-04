     pipeline {
        agent none
        stages {
         
          stage("build & sonarqube") {
            agent any
            steps {
              withSonarQubeEnv('SonarQube_Token') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
