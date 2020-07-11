pipeline {
     agent any
     stages {
         stage('Upload to AWS') {
             steps {
               withAWS(credentials: 'jenkins', region: 'us-west-2') {
                    s3Upload(file:'index.html', bucket:'jspr-project-3-bucket', path:'index.html')
               }
             }
         }
     }
}
