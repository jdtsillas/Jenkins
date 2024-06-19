/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'python:3.12.4-alpine3.20' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'echo "Hello World"'
		        sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''

            }
        }
    }
}
