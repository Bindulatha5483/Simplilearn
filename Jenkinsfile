pipeline {
    agent { label 'slave1' }

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Bindulatha5483/Simplilearn.git'
            }
        }
        stage('Build Stage') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}

