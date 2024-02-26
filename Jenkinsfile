pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggyappp -Dsonar.organization=asgbuggyappp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=10a6f2ecf6250303f7870d493254b914a9ad1d18'
			}
        } 
  }
}
