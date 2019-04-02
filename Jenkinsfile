node {
   def commit_id
   stage('Preparation') {
     checkout scm
   }
   stage('docker build/push') {
     def app = docker.build "srivatsanv1991/srivatsanv:$BUILD_NUMBER"
     docker.withRegistry('', 'docker-hub-cred') {
       app.push()
     }
   }
}