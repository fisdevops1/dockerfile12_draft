pipeline{
    agent any
    stages{
        stage('Stage1 Code Checkout'){
            steps{
                echo 'Automatic Docker Images update'
                checkout scm
            }
        }
        stage('Stage2 Build and Run Tests'){
            steps{
                echo 'mvn clean install'
                echo 'sh java -jar com.test-1.5-SNAPSHOT.jar'
            }            
        }
    }
}