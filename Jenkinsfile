pipeline {
  agent any
  tools { 
        maven 'Maven-3.2.5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-2025 -Dsonar.organization=devsecops-2025 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=0514d8b1a300bd18eb54abb3da1b9ff3e2d98e4b'
			}
        } 
  }
}
