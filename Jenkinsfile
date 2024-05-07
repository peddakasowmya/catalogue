pipeline { 
    agent {
        label 'ws'
    }
    stages {
        stage('Lint Checks') {      // Style checks
            steps {
                sh "echo Installing Lint Checker"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js"
            }
        }
        stage('Static Code Analysis') {     // security code checks
            steps {
                sh "echo Static Checks ...."
            }
        }
    }
}