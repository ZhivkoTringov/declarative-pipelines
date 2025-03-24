pipeline{
    agent any

    stages{
        stage('static-analysis'){
            steps{
                echo 'static-analysis'

                script{
                    def number = input message: "Have you performed static analysis and that has resulted in no High or Critical issues?",
                        parameters: [
                            string(name: 'Value', description: 'Enter a value equally divisible by three.')
                        ]
                    
                    def num = number.toInteger()
                    
                    if (num % 3 ==0){
                        echo "Divisible by three"
                    }else{
                        error "Not divisible by three"
                    }
                }
            }
        }
        stage('build'){
            steps{
                echo 'build'
            }
        }
        stage('unit test'){
            steps{
                echo 'unit test'
            }
        }
        stage('package'){
            steps{
                echo 'package'
            }
        }
        stage('Buld is Successful'){
            steps {
                echo 'Test to Discord'
                discordSend customAvatarUrl: '', customFile: '', customUsername: '', description: 'Build Completed', footer: '', image: '', link: '', result: currentBuild.currentResult, scmWebUrl: '', thumbnail: '', title: 'Build Notification', webhookURL: 'https://discord.com/api/webhooks/1353687249849684039/N3ZHwFoLlPMnFmb8hOEowP-wclDtgewMOkxA8mMxPEWKL-ySw2lJyapBSlCzeZ_wyBWo'
            }
        }
    }
}