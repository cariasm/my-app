pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
        stage('Deploy'){
             steps {
                retry(3) {
                    sh echo "Rety Text"
                }

                timeout(time: 3, unit: 'MINUTES') {
                    sh 'echo "Retry timeoout"
                            }
                        }
                    }
                }
            }