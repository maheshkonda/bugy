pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggyapp -Dsonar.organization=buggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1bb9eed39239ad1587d0cae3e9636e878560b9d0'
			}
        } 
  }
}
