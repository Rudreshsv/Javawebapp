pipeline {
    agent any
        stages {
            stage('checkoutscm') {
                steps{
                 git credentialsId: 'b1ddb61f-a4cf-453f-84a9-022b3e424e43', url: 'https://github.com/Rudreshsv/Javawebapp.git'
                }
            }
            stage('maven build') {
                steps{
                    //cd Javawebapp
                    sh 'mvn clean install'
                }
            }
        }
    }
