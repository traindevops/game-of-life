pipeline {
    agent { label 'master' }
    triggers {
        pollSCM('H * * * 1-5') 
    }
    stages {
        stage('SCM'){
            steps {
                git 'https://github.com/traindevops/game-of-life.git'
            }
        }
        stage('Build'){
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
