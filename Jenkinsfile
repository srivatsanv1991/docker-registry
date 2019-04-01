pipeline{
    agent any
    environment {
        registry = "srivatsanv1991/srivatsanv"
        registryCredential = "docker-hub-cred"
    }
    stages{
        stage('Building Image'){
            steps{
                script{
                   def app= docker.tag("5435658a63ac srivatsanv1991/srivatsanv:latest")
                    app.push("latest")
                }
            }
        }
    }
}
