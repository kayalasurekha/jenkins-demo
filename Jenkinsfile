pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Running Build Stage...'
                sh 'bash app.sh'
            }
        }

    }

    post {
        success {
            echo 'Build SUCCESS ✅'
        }
        failure {
            echo 'Build FAILED ❌'
        }
    }
}
