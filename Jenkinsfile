pipeline {
    agent any 
    stages{
        stage('git Checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/sang2410/fullstack-blog.git'
            }
        }
           stage('Compile'){
            steps{
                script{
                    sh "mvn compile"
                }
            }
        }
        stage('un'){
            steps{
                script{
                    sh "mvn test"
                }
            }
        }
    }
}