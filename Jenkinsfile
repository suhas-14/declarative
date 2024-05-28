pipeline {
    agent any

    stages {
        stage('Fetch the code') {
            steps {
                git 'https://github.com/suhas-14/java-maven.git'
            }
        }
        stage('Build')
        {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Test')
        {
            steps {
                echo 'Testing Phase starts here'
            }
        }
        stage("Results"){
            steps {
                echo "All good"
            }
        }
    }
}
