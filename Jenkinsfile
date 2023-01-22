pipeline {
    agent any
    stages {
        stage(‘git’) {
            steps {
                echo 'this is the git stage to clone the repository'
                git branch: 'master', url: 'https://github.com/sanjayte/JavaRepo.git'
            }
        }
        stage(‘mavenBuild’) {
            steps {
                sh 'mvn clean install'
            }
        }
        stage(‘deploytotomcat’) {
            steps {
                echo 'this is the deploy stage'
            }
        }
        stage(‘test’) {
            steps {
                echo 'this is the test stage'
            }
        }
    }
}
        
