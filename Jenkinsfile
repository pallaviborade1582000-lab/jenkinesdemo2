Pipeline {
    agent any
    environment {
       PYTHON = "C:\\Users\\admin\\AppData\\Local\\Programs\\Python\\Python313\\python.exe"
 
    }
    stages {
        stage('Checkout Code') {
            steps {
                checkout scm
            }

        }
        stage('Extract Data') {
            steps {
                bat "${env.PYTHON} extract.py"

            }
        }
            
    }
    Post {
        success {
            echo "success..."

        }
        failure {
            echo "failure..."

        }
        always {
            echo "Always..."

        }
    }
}