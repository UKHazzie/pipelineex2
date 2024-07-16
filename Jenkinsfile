pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building..."'
                sh 'ls -al'
                sh 'echo "End of Building..."'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Testing..."'
                sh 'pwd'
                sh 'touch testfile.txt'
                sh 'ls -l'
                sh 'echo "End of Testing..."'
            }
        }
        stage('Deploy') {
            steps {
                sh 'cat ./deploy.sh'
                sh 'echo "Deploying..."'
                sh 'mv testfile.txt /tmp'
                sh 'ls -l /tmp'
                sh 'echo "End of Deploy..."'
            }
        }
    }
}
