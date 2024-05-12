pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=john-myfirstproject -Dsonar.organization=john-myfirstproject -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=1dd31553ee6ea7befa132a6bbf24f1d8ce22e02a'
			}
        } 
  }
}
