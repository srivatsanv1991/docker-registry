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
                   docker.withDockerRegistry("https://hub.docker.com/","docker-hub-cred")
                    def app=docker.build("srivatsanv1991/srivatsanv:${commit_id}", '.').push()
                }
                }
            }
        }
    }
}
