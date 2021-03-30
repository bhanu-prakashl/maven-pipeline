pipeline {
    agent any
    environment {
        PATH = "/opt/apache-maven-3.6.3/bin/"
    }
    stages {
        stage("clone code"){
            steps{
               git credentialsId: 'git_credentials', url: 'https://github.com/bhanu-prakashl/maven-pipeline.git'
            }
        }
        stage("build code"){
            steps{
              sh 'mvn clean install'
            }
        }
        
    }
}
