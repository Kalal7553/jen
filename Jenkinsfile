pipeline {
    agent any
    tools {
        maven "maven"
    }
    stages {
        stage ("checkout") {
            steps {
                git branch: 'main', credentialsId: '8f00c1e5-0d58-41a3-8759-8d8e792fe1b2', url: 'https://github.com/Kalal7553/jen.git'
            }
        }
        stage ("build") {
            steps {
                sh "mvn install"
            }
        }
    }
}
