pipeline{
    agent any

    environmet{
        ARTIFACT_SOURCE_DIRECTORY = "test/*.xml"
    }
    stages{
        stage('Build'){
            steps{
                echo 'Build the code'
            }
        }
        stage('Test'){
            steps{
                echo 'Execute unit tests'
                sh 'mkdir -p tests && echo "test results" > tests/testresults.xml'
            }
        }
    }
}