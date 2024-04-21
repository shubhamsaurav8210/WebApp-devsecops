pipeline {
    agent any
    tools {
        maven 'Maven'
    }
    stages {
        stage('Initialize') {
            steps {
                script {
                    // Display the current PATH
                    sh 'echo "PATH = $PATH"'
                    
                    // Display the M2_HOME variable
                    sh 'echo "M2_HOME = $M2_HOME"'
                }
            }
        }

        stage('Build') {
            steps {
                // Run Maven clean and package
                sh 'mvn clean package'
            }
        }
    }
}
