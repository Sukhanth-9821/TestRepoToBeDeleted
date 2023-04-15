pipeline{
	agent any
	tools{
		maven 'maven'
	}
	stages{
		stage("Checkout"){
			steps{
				git branch: 'main', url: 'https://github.com/Sukhanth-9821/docker-Java-kubernetes-project-poc.git'
			}
		}
		stage ("maven build 1"){
            steps{
                sh 'cd productcatalogue'
                sh 'mvn -f productcatalogue/pom.xml clean install package'
            }
        }
		stage ("Docker image build"){
            steps{
                sh 'sudo docker build -t sukhanth/jenkinsfile_jaja_k8s:latest ./productcatalogue'
                // sh '$images = sudo docker images'
                // sh 'echo $images'
            }
        }
		
		
		
	}


}
