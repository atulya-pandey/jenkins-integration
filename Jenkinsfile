pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
        
        stage('list buckets') {
            steps {
                sh 'aws s3 ls'
            }
        }
    }
}