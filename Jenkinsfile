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
                   dockerBuildAndPublish {
            repositoryName('srivatsanv1991/srivatsanv')
            tag('${GIT_REVISION,length=9}')
            registryCredentials('docker-hub-cred')
            forcePull(false)
            forceTag(false)
            createFingerprints(false)
            skipDecorate()
                }
            }
        }
    }
}
