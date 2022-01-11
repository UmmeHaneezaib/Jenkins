pipeline {
    agent any
    tools {
        maven 'MAVEN'
    }

    stages {

        stage('Build Maven') {
            steps{
                 git branch: 'main', credentialsId: 'UmmeHaneezaib', url: 'https://github.com/UmmeHaneezaib/Jenkins.git'
                 sh "mvn -Dmaven.test.failure.ignore=true clean package"
                
            }
        }  
    }
}
