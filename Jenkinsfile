pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp3 -Dsonar.organization=asgbuggywebapp3 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=9325586a8f1d1adf470b908a46156f5844'
			}
        } 
  }
}
