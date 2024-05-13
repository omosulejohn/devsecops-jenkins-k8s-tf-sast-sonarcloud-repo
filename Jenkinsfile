pipeline {
    agent any
    tools {
        // Define the Maven tool
        maven 'Maven_3_5_2'
    }
    stages {
        stage('Compile and Run Sonar Analysis') {
            steps {
                // Execute Maven commands
                script {
                    sh 'mvn verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=johnwebapp2'
                }
            }
        }
    }
}
