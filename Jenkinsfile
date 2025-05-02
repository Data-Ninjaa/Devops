pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                 git branch: 'main', url: 'https://github.com/Data-Ninjaa/Devops.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Run Python Script') {
            steps {
                echo 'Running Python file...'
                sh 'python3 hello.py'   // <-- change "script.py" to your actual filename
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
