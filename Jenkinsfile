#! /usr/bin/env groovy

pipeline {
    agent {
        docker {
            image 'maven:3.8'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh './scripts/build.sh'
            }
        }
    }
}