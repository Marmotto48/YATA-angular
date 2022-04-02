pipeline {
    agent any

    stages {
        stage('npm install') {
            steps {sh "npm install"
                echo 'ess..'
            }
        }
        stage('run') { 
            steps{script{
                withEnv(['BUILD_ID=dontkill']) {
                     sh "ng serve &"
                }
            }
                }
        }
        steps {script{
                withEnv(['BUILD_ID=dontkill']) {
                     sh "ng serve &"
                }
            }}
        }

        }
