pipeline {
    agent any

    stages {
        stage('Git pull source code'){
            steps {
                git branch: 'main', url: 'https://github.com/adelochea/sample-repo.git'
            }
        }
        
        stage('Build source'){
            steps {
                bat ''' cd /C C:\\jenkins\\jenkinslocalgit
                npm install '''
            }
        }
        stage('Testing') {
            steps {
                echo 'Testing Completed'
            }
        }
        stage('Release') {
            steps {
                echo 'Release Done'
            }
        }
    }
}
