pipeline{
    agent any
    tools{
        maven 'maven-3.9.9'
    }
    stages{
        stage('Maven version'){
            steps{
                sh 'mvn --version'
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