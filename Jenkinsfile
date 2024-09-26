pipeline {
    agent any
    tools{
        maven 'Maven'
    }
    stages{
        stage('Build Maven'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/TANZID36/jenkins-project']])
                sh 'mvn clean install'
            }
        }
    }
}
