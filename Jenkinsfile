pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sonar-sast-demo -Dsonar.organization=sonar-sast-demo -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=8450a12e7a0e3c853702b9eb7867aed6da7ddfe1'
			}
        } 
  }
}
