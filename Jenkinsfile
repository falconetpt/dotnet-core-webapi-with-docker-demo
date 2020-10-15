pipeline {
    agent any
    stages {
        stage("Checkout") {
            steps {
                git url: 'https://github.com/falconetpt/dotnet-core-webapi-with-docker-demo', branch: 'master'
            }
        }
    }
}