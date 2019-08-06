pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(credentials:'aws-static') {
              s3Upload(file:'file.txt', bucket:'my-bucket', path:'index.html');
            }
      }
    }
  }
}
