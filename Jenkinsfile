pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=p_devsecops_webapp -Dsonar.organization=p_devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=519bdd08b9fe98854a40dd64effd0b0f9cdfba1d'
			}
        } 
  }
}
