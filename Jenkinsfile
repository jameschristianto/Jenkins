node {
    agent any
    triggers { 
        pollSCM('H/2 * * * *') 
    }
    stage('Build') {
        sh 'npm install'
    }
    stage('Test') {
        sh './jenkins/scripts/test.sh'
    }
}