pipeline {
    agent any
    stages {
        stage("Checkout") {
            steps {
                git url: 'https://github.com/falconetpt/dotnet-core-webapi-with-docker-demo', branch: 'master'
            }
        }
       stage("run app") {
        steps {
            sh 'docker build .'
            sh 'docker run -t -p 1234:5000 dotnetapidemo'
        }
       }
    }
}