pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Start Building..."'
                sh './building.sh'
                sh 'echo "End of Building..."'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Start Testing..."'
                sh './testing.sh'
                sh 'echo "End of Testing..."'
            }
        }
        stage('Deploy') {
            steps {
                sh 'cat ./deploy.sh'
                sh 'echo "Start Deploying..."'
                sh './deploying.sh'
                sh 'echo "End of Deploy..."'
            }
        }
    }
}
