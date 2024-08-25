pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devwebapp -Dsonar.organization=devwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6577d92cb810fde49db6658c667b1a842ad1a4af'
			}
        } 
  }
}
