node {
    try {
        stage('Checkout Code') {
            checkout scm

        }
        stage('Extract Data') {
            bat "C:\\Users\\admin\\AppData\\Local\\Programs\\Python\\Python313\\python.exe extract_data.py"

        }
    }
    catch(err) {
        echo "Pipeline Error : ${err}"
    }
    finally {
        echo "Pipeline completed"
    }
}