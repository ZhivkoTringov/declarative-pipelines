pipeline {
    agent any
    
    stages {
        stage('SCM'){
            steps {
          	   git branch: 'main', credentialsId: '1112', url: 'git@github.com:ZhivkoTringov/declarative-pipelines.git'
            }
        }
    }
}
