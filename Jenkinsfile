pipeline { 
 agent any
 stages {
    stage('Fetch code') {
        steps {
            git branch: 'paac', url: 'https://github.com/582Bamfo/vprofile-project.git'
    }
 }
 stage('build'){
    steps {
        sh 'mvn install'
    }
 }
 stage('Test'){
    steps {
        sh 'mvn test'
    }
 }
}
}