#!groovy

pipeline {
    agent any

    stages {
        stage("Preparing"){
            steps{
                echo "Hello World!"
            }
        }
        stage('Test PetStore collection') {
            steps {
                echo "Start testing"
                bat "newman run PetStore.postman_collection.json"
                echo "Finish testing"
            }
        }
    }
}
