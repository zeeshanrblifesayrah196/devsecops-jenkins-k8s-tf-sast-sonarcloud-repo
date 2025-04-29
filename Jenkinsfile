pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=zrbDevsecopsBuggyWebapp -Dsonar.organization=zrborganization -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=4a625340b85358bda66bf66e06433ed4307f6f7f'
			}
        } 
  }
}
