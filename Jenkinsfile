pipeline {
     agent { label 'master' }
     stages {
         stage('Build') {
             steps {
                 echo 'Building...'
             }
             post {
                 always {
                     jiraSendBuildInfo site: 'asthaopendeveops.atlassian.net'
                 }
             }
         }
     }
 }
