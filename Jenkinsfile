pipeline {
  agent {
    kubernetes {
      label 'mypod'
      defaultContainer 'jnlp'
      yamlFile 'pod.yaml'
    }
  }
  stages {
      stage('Run maven') {
				steps {
					 container('maven') {
						  sh 'mvn -version'
					 }
					 
				}
		  }
	 }
}
