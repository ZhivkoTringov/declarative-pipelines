pipeline {
    agent any
    
    environment {
        SENTENCE = " What are you think you are doing?"
    }
    stages {
        stage('Hello'){
            steps {
                echo 'Hello World!'
                
                script {
                    def words = env.SENTENCE.split(' ')
                    
                    for (word in words){
                        echo word
                    }
                }
            }
        }
    }
}
