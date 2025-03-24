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
                discordSend customAvatarUrl: '', customFile: '', customUsername: '', description: 'Build is Successful', footer: '', image: '', link: '', result: '', scmWebUrl: '', thumbnail: '', title: '', webhookURL: 'https://discord.com/api/webhooks/1353681555716964432/Bd-e5dQbBGBnAT1syqvdxUjgju6B2OwZBQ7nsWrOgabr04wlwjhPzTWI2M2qzwOKXnMP'
            }
        }
    }
}