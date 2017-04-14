#!groovy

stage('Pull') {
    node {
        git credentialsId: 'e921f6be-72bb-44bd-aca4-7a87f6a581d2', url: 'git@github.com:playground-io/prometheus.git'
    }
}

stage('Deploy Whitebox Monitoring') {
    node {
        bat 'docker-compose up'  
    }
}