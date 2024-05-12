pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=john-myfirstproject -Dsonar.organization=john-myfirstproject -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=17ab71908303b91dd280ed9074ba1f55b797d7ff'
			}
        } 
  }
}
