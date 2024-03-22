pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Validation') {
            steps{
                script{
                    if(params.build){
                    echo " We will build the project.. "
                    sh 'ls'
                    sh 'if [ -d "test" ]; then rm -r test ; fi'
                    sh 'mkdir test'
                    dir('test'){
                    sh 'ls' }
                    }
                }
            }
        }
        stage('t') {
            steps {
                script {
                    sh 'ls'
                }
            }
        }
    }
}
