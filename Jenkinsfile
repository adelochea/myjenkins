pipeline {
    agent any

    stages {
        stage('Git pull source code'){
            steps {
                git branch: 'main', url: 'https://github.com/adelochea/sample-repo.git'
            }
        }
        
        stage('Compile source code'){
            steps {
                bat ''' cd /C C:\\jenkins\\jenkinslocalgit
                npm install '''
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
