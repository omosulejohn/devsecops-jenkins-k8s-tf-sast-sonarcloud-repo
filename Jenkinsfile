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
                    sh 'mvn clean verify sonar:sonar \
                        -Dsonar.projectKey=johnwebapp2 \
                        -Dsonar.organization=johnwebapp2 \
                        -Dsonar.host.url=https://sonarcloud.io \
                        -Dsonar.login=8b586880c918d9a5f87982bdadf3cf8348c44a17'
                }
            }
        }
    }
}
