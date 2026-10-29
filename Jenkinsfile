pipeline {
    agent any
    stages {
        stage("Checkout") {
            steps {
                checkout scm
            }
        }
        stage("Run Application") {
            steps {
                bat "python hello.py"
            }
        }
        stage("Run Tests") {
            steps {
                bat "python -m pytest -v"
            }
        }
    }
}
