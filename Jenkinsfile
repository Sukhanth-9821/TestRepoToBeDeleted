pipeline{
    agent any
    tools{
        maven 'maven'
    }

    // environment{
    //     DOCKERHUB_USERNAME = credentials('')
    // }
    stages{
        stage('Checkout'){
            steps{
            git branch: 'main', url: 'https://github.com/Sukhanth-9821/docker-Java-kubernetes-project-poc.git'
            }
        }
		}
        
}
