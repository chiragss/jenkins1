pipeline {
    agent any

    stages {
        stage('Setup Virtual Environment') {
            steps {
                sh 'pip install virtualenv'
                sh 'python -m virtualenv venv'
                sh '. venv/bin/activate'
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Python Code') {
            steps {
                sh 'python sample.py'
            }
        }

        stage('Deactivate Virtual Environment') {
            steps {
                sh 'deactivate'
            }
        }
    }
}

