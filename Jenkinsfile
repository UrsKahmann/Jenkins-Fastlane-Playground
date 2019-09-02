pipeline {
    agent any

    stages {
        stage('Setup') {
            steps {
                echo 'Building..'
                script {
                    stage('Playing around') {
                        sh '''
                            #!/bin/bash -l
                            cd fastlane
                            bundle install
                            bundle exec fastlane setup '''
                    } 
                }
            }
        }
        stage('Build') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}