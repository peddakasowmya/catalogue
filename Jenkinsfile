@Library('shared-library') _



pipeline { 
    agent {
        labels 'ws'
    }
    stages {
        stage('Lint Checks') {      // Style checks
            steps {
                nodejs.lintChecks()
            }
           /* 
            steps {
                script {
                    sample.info('Ola')
                }
                sh "echo Installing Lint Checker"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js || true"
            }*/
        }
        stage('Static Code Analysis') {     // security code checks
            steps {
                sh "echo Static Checks ...."
            }
        }
    }
}
 
 