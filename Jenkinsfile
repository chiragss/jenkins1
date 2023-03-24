pipeline {
    agent any

    stages {
        stage('Setup Virtual Environment') {
            steps {
                sh 'pip install virtualenv'
                sh 'python3 -m virtualenv venv'
                sh '. venv/bin/activate'
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Python Code') {
            steps {
                sh 'python3 sample.py'
            }
        }

        stage('Deactivate Virtual Environment') {
            steps {
                sh 'https://github.com/chiragss/jenkins1.git'
		sh 'exit'
            }
        }
    }
}

